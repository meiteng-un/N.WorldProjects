# PlayMode性能診断・範囲休止設計（2026-10-12）

## 対象と保護

対象: N.Worlds Project -001。ユーザーがConsole消去後、PlayMode診断・改善を依頼。YamaStreamは変更しない。元Sceneの保存、購入アセットの削除・一括停止、権限設定変更は行っていない。

## 実測

初回ポイント測定: 約4FPS、264ms/frame、Renderer 3965、active GameObjects 9608。

30秒の起動直後計測（Profiler有効、ClientSim通常ログのみ一時OFF）:

|項目|通常GameView|GameView一時最大化|
|---|---:|---:|
|FPS|3.00|3.22|
|Main Thread (ms)|327.371|308.581|
|PlayerLoop (ms)|72.660|70.689|
|Camera.Render (ms)|30.680|31.078|
|Physics.Simulate (ms)|5.024|4.844|
|Udon ManagedUpdate (ms)|15.850|14.667|
|Udon ManagedLateUpdate (ms)|0.348|0.341|
|Udon ManagedFixedUpdate (ms)|1.520|1.437|
|Udon PostLateUpdate (ms)|0.147|0.138|
|Gfx.WaitForPresentOnGfxThread (ms)|0.737|0.035|

Render Threadは取得不可。EditorLoop、WaitForTargetFPSは0だが、待機やEditor処理が存在しない証明ではない。マーカーには包含関係がある。Udonの遅延イベント・ネットワークイベント・初期化等すべての実行時間を網羅した計測ではない。最初の30秒には初期化が含まれる。前面/バックグラウンド条件の記録がなく、通常と最大化の差を改善率として扱わない。

ログOFFだけでも低FPSが継続。計測した更新処理だけではフレーム全体の時間を説明できない。主原因の確定・恒常的な性能改善は未完了。

## 新しいログの分類

- TMP下線文字不足: 多くはAwake時。TMP_ItemNameの絵文字不足も発生。
- MirrorController OnValidate警告、Missing Script、SDKのPrefabBuild/Scene前処理: 起動時/Editor側の問題として区別。
- ClientSim EditorOnly削除ログ: 起動時。累積件数だけで毎フレーム負荷とは判断しない。
- SignPlateの同期方式競合: 同期リスク。今回修正していない。
- YamaStream: 依頼どおり動作コード・設定変更なし。計測中のerror件数には含まれる。
- PlayMode終了後のAsset Garbage Collect: 約36秒、約35秒がDeleteObjects。これはプレイ中の恒常的FPSと別問題。

## 追加した計測ツール

`Assets/N.Assets/Editor/NPlayModePerformance.cs`（既存のimport済みEditor配置を利用）。

Tools/Naturlin/Performance以下:
- Measure Baseline (30 seconds)
- Measure Quiet ClientSim (30 seconds)
- Measure Quiet Maximized GameView (30 seconds)

明示的に開始。PlayMode開始後30秒でTempレポートを書き、ログ設定・Profiler有効状態・GameView最大化状態を復元してPlayMode終了。ClientSimのグローバルEditorPrefsは保存しない。途中終了/アセンブリ再読み込み時もCleanupで復元。

初期の計測コードは容量1のバッファの上書き設定漏れで時間がすべて0だったため、その時間内訳は無効。Unity 2022.3の列挙値名の誤記による一時的C#エラーも修正済み。上表は `WrapAroundWhenCapacityReached` 修正後の値。

## 次の切り分け

Unityを前面に置き、同じ位置・同じ描画条件で計測する。Editorのバックグラウンド更新制限、PlayerLoop外の時間、Render Thread/GPUの詳細、Udon遅延イベント等を追加確認する。必要ならUnity ProfilerのCPU Timelineを使用。現段階でUdonの大量配置だけを主原因として扱わない。

## 範囲外休止の構想

有効になり得るが、対象負荷により効果は異なる。まず設計案として保管し、全ギミックへの適用は未実施。

- 部屋/階単位の少数の管理処理で切り替える。全ギミックの毎フレーム距離判定は避ける。
- 表示・演出・周辺判定と、重要な同期・所有権・共有状態を分離する。
- 復帰方針をギミックごとに選択: 続行／保存状態復元／初期化。
- 育成・栽培等は最終更新時刻と状態を保持し、復帰時に時間差分を反映する。
- 魚・装飾・ローカルUIは周辺プレイヤー不在時に更新・描画を休止する候補。
- エレベーター・共有機械は所有者と利用者の存在を考慮。自分が遠いだけで共有処理を止めない。
- 初期化イベントは再入場ごとにStartが再実行される前提にしない。重複する遅延イベントの再スケジュールも防ぐ。
- disabledなUdonBehaviourもネットワークイベントの対象になり得るため、enabled=falseだけで全Udon処理停止を保証しない。

## 公式参照

- [ProfilerRecorder](https://docs.unity3d.com/2022.3/Documentation/ScriptReference/Unity.Profiling.ProfilerRecorder.html) — Unity 2022.3のマーカー計測とリソース解放。
- [ProfilerRecorderOptions](https://docs.unity3d.com/2022.3/Documentation/ScriptReference/Unity.Profiling.ProfilerRecorderOptions.html) — サンプル容量超過時の上書き設定。
- [VRChat Network Events](https://creators.vrchat.com/worlds/udon/networking/events/) — disabledなBehaviourへのイベント送信。
- [Network Variables](https://creators.vrchat.com/worlds/udon/networking/variables/) — 途中参加時に必要な共有状態。
