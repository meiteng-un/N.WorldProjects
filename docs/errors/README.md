# Error Records

エラーの再現条件、原因候補、修正、検証結果を記録します。

## 記録テンプレート

コピーして `docs/errors/YYYY-MM-DD-short-name.md` として保存します。

```md
# [Bug] 短いタイトル

- Status: 未確認 / 調査中 / 修正案 / 検証待ち / 完了
- Date:
- Project:
- Scene:
- Prefab/GameObject:
- Script/Asset:

## 症状

## 再現手順

1.
2.
3.

## 期待する動作

## 実際の動作

## ログ・証拠

## 原因候補

## 修正内容

## 検証

- [ ] ソース確認
- [ ] Unity Refresh/Compile
- [ ] Console確認
- [ ] Scene/Prefab保存と参照再確認
- [ ] PlayMode
- [ ] VR/Desktop入力
- [ ] VRChat実機・複数ユーザー

## 未確認事項

## 関連Issue/PR
```

原因が未確定の場合は、仮説として記録し、確認済みの事実と分けてください。
