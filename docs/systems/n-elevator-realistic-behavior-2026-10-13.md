# N.ElevatorSystem 改善記録（2026-10-13）

## 現在の構成・問題
- 実際のSceneは52ボタンを持つ親Manager 1個。Desktopは独自Raycast＋InputUse。DisableInteractiveのためVRChat標準Use表示は出ない。
- エラーClipが未設定だった。購入済みエレベーターのSwitch_error.wavを欠落箇所にのみ設定する補助を追加。
- AのかごAnimatorはMESH、BはElevator_Anim。Aの左右ドアはGondolaの子。AのドアCurveパスは一致、AnimatorはAlwaysAnimate・有効、左右ドアのStaticフラグは0。7F以外で動かない根本原因は未確定。BとVRは未確認。

## 変更
- 近接による扉操作を廃止。乗り場Call／かごOpenで開く。
- 到着・全開後の待機を35秒に設定。途中の行先追加で待機を取消さない。Close操作は待機を早送りし、閉じ切ってから次の要求へ進む。
- 行先要求中の発光を保持し、到着で要求解除後に消灯色へフェード（既定0.8秒）。
- Desktopに独自の視線ハイライトと[Use / LMB]案内を追加。標準VRChat Interact表示そのものではない。壁越しの操作は許可しない。
- エラー音の欠落補完と共通案内TextMeshProを設定するEditor補助を追加。バックアップ・Undo付き、元Sceneは自動保存しない。

## 検証・未確認
ソース変更とScene調査の記録。最終コンパイル・設定適用結果はローカル記録に追記する。Aの到着階ドア、Desktop実操作、権限拒否の音と赤点灯、35秒待機・Close早送り・多人数同期・B・VRは実機検証を要する。PlayMode性能改善は保留。安全センサーや方向別配車などは今回未実装。

## 最終適用確認
- UdonSharp 1,368スクリプトの最終コンパイル完了（63.142秒）。Use案内のProgram定義反映を確認し、対象2 Program Assetのみ保存。
- Sceneで待機35秒、Use案内参照、ManagerのSwitch_error参照を確認。新規Program反映後にSystemとManagerのProxy参照を再転送した。元Sceneは未保存。
- バックアップ: Temp/N_ElevatorRealistic_20261013_152351_958.unity。途中で検出したTMP_Text.transformの未公開APIはgameObject.transformへ修正済み。途中のエラーログはConsoleに履歴として残り得る。
- AのパラメーターDoorStateとSystem設定は一致し、A配下に有効な旧Udonは見つからなかった。ドア不動の解決は引き続き未確認。
