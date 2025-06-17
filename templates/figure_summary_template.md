---
title: Figure ごとの実験内容と結果の要約
description: 各 Figure について、目的・手法・結果・解釈の順で整理してください。
tags: [summary, figure, cursor-workflow]
---

## 📂 対象論文ファイルのパス

[`summaries/papers/論文ファイル名.md`](../summaries/papers/論文ファイル名.md)

## 📌 タスク

1. 対象論文の各 Figure に対応する説明文を読み取ってください。
2. 各 Figure について以下の項目を日本語で記述してください：
   - 実験の目的
   - 使用した手法
   - 得られた主な結果
   - 結果の解釈・意義
3. 出力は `summaries/figure_summaries/論文ファイル名_figure_summary.md` に保存してください。
4. **画像（Markdown 形式の `![](https...)`）は同じ位置で表示されるようそのままコピーして挿入してください。**
5. 出力内のファイルリンク（例：`[元論文を開く](../papers/論文ファイル名.md)`）は、  
   **スペースを `%20` に変換したエンコード形式**で記述してください。

例：  
`A vagus nerve dominant tetra-synaptic ascending pathway.md`  
→ `A%20vagus%20nerve%20dominant%20tetra-synaptic%20ascending%20pathway.md`

## 🧾 出力フォーマット（コピーして編集）

```markdown
---
source: 20_Literature/論文ファイル名.md
summary-date: 2025-06-15
type: figure_summary
---

> 🗂 [元論文を開く](../papers/論文ファイル名.md)

## 各 Figure の要約

### Figure 1

- 実験の目的：
- 使用した手法：
- 得られた主な結果：
- 結果の解釈：

![](https://example.com/fig1.png)

### Figure 2

- 実験の目的：
- 使用した手法：
- 得られた主な結果：
- 結果の解釈：

![](https://example.com/fig2.png)

...
```
