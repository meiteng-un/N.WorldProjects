# World / Avatar 境界と担当運用

## 保存先
- Avatar: https://github.com/meiteng-un/N.AvatarProjects
- Unity Avatar: D:\VCCUnity\VRChatProjects\N.Avatars Project
- Web ChatGPT Avatar: https://chatgpt.com/g/g-p-6acf92412d1c8191b0eee4feb66485a4/project
- World: https://github.com/meiteng-un/N.WorldProjects
- Unity World: D:\VCCUnity\VRChatProjects\N.Worlds Project
- Web ChatGPT World: https://chatgpt.com/g/g-p-6acbb380b0e88191967db66da351c0d4/project

相手のリポジトリは調査のために読むことができる。知見は出典のURL・commit・適用理由を記録して参照する。相手の文書、Issue、画像、Material、Prefab、Scene、Scriptを自動コピーしない。各成果物、ログ、決定、PRは対象側に保存する。共有する概念も対象側に適合するか確認する。転用が必要な場合はユーザーの明示指定、ライセンス、依存関係を確認してから対象側の独立した変更として扱う。

## 担当
- ユーザー: イメージ、制約、参考画像、採用判断を伝える。
- 司令塔 Codex: 対象判定、依頼の具体化、担当割当、GitHub記録、統合レビュー。
- 調査・デザイン担当: 出典、見た目、仕様、受入条件を整理する。
- 実装担当: 対象Unity/Blenderで変更し、変更箇所と検証証拠を戻す。
- Web ChatGPT担当: 画像付きプロンプトを受けて画像生成・見た目の提案を行う。
- 検証・報告担当: 実施済みチェックと未確認事項を区別する。

役割は責任の分担であり、全員を常時別チャットや別エージェントで起動しない。小規模な設定・修正・Unity操作は司令塔が担当する。独立した大きな作業のみ狭い範囲で委任し、同じファイルやUnity接続先には一人の書き手を割り当てる。既存の別チャットへの送信はユーザーの送信許可がある場合に行う。

## GitHubの進行
対象リポジトリにIssueまたは docs/tasks/<task-slug>/brief.md を作成し、目的、対象パス、参照画像、制約、受入条件を記録する。実装は対象側のブランチとPRで管理する。report.md に変更、画像生成履歴、検証、残課題を記録する。Unity全体や購入アセットを自動アップロードしない。ローカルUnityプロジェクトとGitHub文書リポジトリは別物として扱う。

## 画像生成とWeb ChatGPT
Avatar改変のMatCap、Base Color、PBR用画像、Normal、Maskなどはアバター用サイドパネルChatGPTを優先する。ユーザーの曖昧なイメージを、用途・色・質感・形・変更対象・保持条件・解像度・透過・タイル性・納品物まで具体化する。ユーザーが提供または送信を許可した対象画像を添付し、画像ごとの役割を明記してプロンプトと一緒に渡す。対象画像がなければ画像添付済みと記録せず、依頼文の準備段階とする。

World用チャットへAvatar画像を送らず、Avatar用チャットへWorld画像を送らない。開いているURLとプロジェクト名を送信前に確認する。ブラウザが利用できない場合は失敗を報告し、プロンプトを保存する。別の生成方法へ無断で切り替えない。受信した提案は司令塔が検証し、Unity適用をWeb回答だけで完了扱いしない。

生成画像は候補として扱う。PBR各マップの整合性、Normalの向きと凹凸、UV一致、シーム、解像度、alpha、実ファイルを確認する。Normal画像は必要に応じて高さ情報から変換し、生成された青紫の画像だけで正しい法線と判断しない。色空間、Normal Map指定、圧縮、shaderのチャンネル配置は実際のshaderとUnity設定で確認する。

## 検証
資料の作成、生成画像の取得、Unity import、Material適用、保存済みPrefab/Scene、PlayMode、VRChat実機を個別に記録する。実行していない段階は未確認とする。
