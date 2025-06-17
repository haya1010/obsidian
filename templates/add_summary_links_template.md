---
title: 元論文への要約リンク付与
description: 元論文ファイルに各種要約へのリンクを追加するためのテンプレート
tags: [summary, link, cursor-workflow]
---

## 📂 対象論文ファイルのパス

[`summaries/papers/論文ファイル名.md`](../summaries/papers/論文ファイル名.md)

## 📌 タスク

1. 元論文ファイルの先頭（YAML frontmatter の直後）に以下のリンクセクションを追加してください。
2. 各リンクは、対応する要約ファイルへの相対パスで記述してください。
3. ファイル名にスペースが含まれる場合は、**スペースを `%20` に変換したエンコード形式**で記述してください。

例：  
`A vagus nerve dominant tetra-synaptic ascending pathway.md`  
→ `A%20vagus%20nerve%20dominant%20tetra-synaptic%20ascending%20pathway.md`

## 🧾 追加するリンクセクション

```markdown
## 📚 関連要約

- [📊 Figure ごとの要約（パネル説明を含む）](../fig_summaries/論文ファイル名_fig_summary.md)
- [📝 Figure ごとの実験内容と結果の要約](../figure_summaries/論文ファイル名_figure_summary.md)
- [📖 驚き屋風ストーリー型論文要約](../story_summaries/論文ファイル名_story_summary.md)

---
```

## 📝 注意事項

1. リンクセクションは、YAML frontmatter の直後（最初の見出しの前）に配置してください。
2. 各リンクは、対応する要約ファイルが存在する場合のみ追加してください。
3. ファイル名のエンコードを忘れずに行ってください。
4. セクションの前後に空行を入れて、可読性を確保してください。
