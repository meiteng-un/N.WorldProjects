# External References

公開GitHubや公開ドキュメントを、設計比較・API確認・実装方針の参考にするための記録です。

- [目的別参考URL一覧](reference-links.md)

## 必須項目

各外部参考には次を記録します。

- Repository or document URL
- 取得日
- 対象のブランチ、タグ、コミット
- ライセンス
- 参照したファイル・セクション
- N.WorldProjectsでの用途
- 採用した考え方と、採用しなかった部分
- ソースやアセットをコピーしたか
- NOTICE、フォント、画像、依存ライセンスの確認状況
- 次回更新時の確認事項

## Discovery and quality filter

X、Chrome、GitHub検索などで候補を見つけた場合も、次の条件を確認してから一覧へ追加します。

- N.WorldsのUI、UdonSharp、VRChat World、性能、検証に直接関係する
- READMEだけでなく、実装構成、更新状況、Issue/PR、互換性を確認できる
- LICENSE、NOTICE、フォント、画像、第三者依存の条件を確認できる
- 採用する場合の導入方法と、既存システムとの競合が判断できる
- 「参考のみ」「候補」「採用済み」を明確に分けられる

品質を確認できないリンクは、人気や投稿時期だけを理由に登録しません。

## 利用方針

1. まずREADME、LICENSE、NOTICE、package manifestを確認する。
2. 必要な箇所だけを読み、リポジトリ全体を無条件に取り込まない。
3. 参考・設計影響・コード流用を明確に区別する。
4. コードやアセットを流用する場合は、ライセンス条件と帰属表示を対象ファイルの近くにも残す。
5. 公開情報であっても、個人情報、秘密情報、非公開Issueの内容は保存しない。
6. 外部の実装を採用しても、Unity/UdonSharp/VRChat上の動作検証はN.WorldProjects側で別途行う。

## ステータス

- **Reference only**: 比較・設計の参考のみ
- **Candidate**: 採用可能性を調査中
- **Adapted**: ライセンスを確認して一部を適応
- **Adopted**: 採用と検証が完了
- **Rejected**: 条件・性能・互換性などの理由で不採用