---
title: 論文データベース登録テンプレート
description: 論文メタデータ（YAML）からデータベース行を生成します
tags: [database, metadata, paper-index, cursor-workflow]
---

## 📂 対象ファイル

例：`papers/A_vagus_nerve_dominant_tetra-synaptic_ascending_pathway_for_gastric_pain_processing.md`

---

## 📌 タスク

次の項目を YAML メタデータから抽出し、Markdown テーブル形式で出力してください：

- `title`: 論文タイトル
- `author`: 最後の著者名を `Lab名` として使用
- `published`: 発表年（例：2024）
- `source`: 論文元リンク
- 各種リンク（論文本体、パラグラフ要約、図要約）を以下のパスに基づいて出力：

| カラム         | パス                                                            |
| -------------- | --------------------------------------------------------------- |
| 論文本体       | `papers/ファイル名.md`                                          |
| Paragraph 要約 | `summaries/paragraph_summaries/ファイル名_paragraph_summary.md` |
| Figure 要約    | `summaries/fig_summaries/ファイル名_fig_summary.md`             |

---

## 🧾 出力フォーマット（コピーして使用）

```markdown
| タイトル                             | 研究室 | 発表年 | ジャーナル   | 本文                            | Paragraph 要約                                                                     | Figure 要約                                                         | Paragraph 要約完了 | Figure 要約完了 |
| ------------------------------------ | ------ | ------ | ------------ | ------------------------------- | ---------------------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------ | --------------- |
| [論文タイトル](papers/ファイル名.md) | Lab 名 | 発表年 | ジャーナル名 | [📄 本文](papers/ファイル名.md) | [📝 Paragraph 要約](summaries/paragraph_summaries/ファイル名_paragraph_summary.md) | [📊 Figure 要約](summaries/fig_summaries/ファイル名_fig_summary.md) | ❌                 | ❌              |
```

出力されたテーブル行は `database/papers_db.md` に追加してください。
