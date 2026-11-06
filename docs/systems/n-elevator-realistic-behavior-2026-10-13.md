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

## VRChat実機報告に基づく追加改善
- 実機報告: Desktop操作は良好。外側の扉は動作し、かご側は7Fのみ動作。案内の埋没、開閉ボタンの待機誘導色、待機階での常時開放、Desktop押込なしを確認（ユーザー報告）。
- かご扉をAnimatorから同期状態に基づくローカル座標制御へ変更。既存Close/Open ClipからA/B各左右の座標を抽出し、開閉時間に合わせて補間する。4枚の移動量は各約0.7159。かごAnimatorのみ無効化、外側のAnimatorは維持。元の7F限定動作の根本原因を特定したとは主張しない。
- 開始時は閉扉。呼出／Openで開き、全開後35秒で次の要求の有無に関わらず閉じる。Closeは待機を省略する。
- Use案内は視点とボタンの間へ表示し、近いボタンでは距離を縮め、見かけの大きさを維持。Open／Close／Call／Floorと階名を表示する。標準Interact表示ではない。
- 開閉ボタンの待機時は消灯。視線対象のハイライトと押下中発光は保持する。
- Desktopは設定した軸・押込距離へ移動し、desktopPressHoldDuration（既定0.12秒）後に元へ復帰。VRは指の深さに追従する。
- 検証: UdonSharp 1,368スクリプト完了（58.512秒）、新規Program定義反映、Scene内の扉4枚と開始時閉扉を確認。外側Animatorの無効数0、最新Consoleエラー0。対象2 Program Assetのみ保存。元Sceneは未保存。
- バックアップ: Temp/N_ElevatorRealistic_20261013_235033_268.unity。保存に時間がかかりHTTP応答がタイムアウトしたが、その後の読取で適用を確認。Undoも保持。
- 残検証: 新方式でのR/7F/B2到着扉、VR/Desktop押込、案内可読性、35秒待機とClose、途中反転、所有者交代・途中参加・多人数。安全センサーや方向別配車は未実装。
