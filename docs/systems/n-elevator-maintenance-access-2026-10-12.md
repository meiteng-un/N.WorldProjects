# N.ElevatorSystem メンテナンス例外（2026-10-12）

PlayMode性能改善は保留のまま。既存メンテナンスモードを拡張し、モード切替とモード中の操作権限をSystem側で判定する。

- worldCreatorNames / maintenanceExceptionNames に登録した表示名はメンテナンス操作を許可。
- N.Authority Level_Manager の数値権限（individualUserNames / individualUserAuthorityLevels、ローカルデバッグ上書き）を参照。グループ役職名とは区別。
- maintenanceMinimumAuthorityLevel は既定6、設定可能0〜6。未登録・参照欠落は拒否する。
- メンテナンスONかつ許可ユーザーなら運行許可OFFスロットと非アクティブな乗り場でも移動可能。配列外スロット、停止座標欠落/非アクティブ、かご・移動範囲欠落は引き続き拒否。
- 製作者でもメンテナンスOFF時は運行許可OFF階へ行けない。床・出口・衝突安全性は製作者の確認が必要。この例外は建設・整備用であり、安全な一般公開乗り場を保証しない。
- ボタンから渡されたprivilegedだけでメンテナンス権限を通過させない。移動要求とモード切替はSystemでローカルユーザーを確認する。
- authorityLevelManager未設定ならStartで専用名のGameObjectから1回だけ解決する。手動参照は上書きしない。

検証: C# DLL更新、1368 UdonSharpスクリプト完了（58.347秒）、maintenanceMinimumAuthorityLevelのProgram定義反映、最新Consoleエラー0を確認。対象Programのみ保存、元Sceneの自動保存なし。実機・多人数・所有者交代・建設階の床は未検証。

未完了: 先に依頼されたNElevatorButtonsManagerへの改名、標準の親管理、行形式Inspector、材質スロット選択、近接時開放/無人閉鎖、階別の一般利用条件UI、指定ワールドオーナーの一般権限ポリシー。現在の旧無人再開放動作はまだ置換していない。
