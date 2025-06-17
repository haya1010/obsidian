---
title: 論文要約ワークフロー
description: 指定した論文.mdから要約を生成し、summaries/に保存する
tags: [summary, automation, cursor-workflow]
---

## 対象論文ファイルのパス

`papers/論文ファイル名.md`

## 📌 タスク

以下の手順で要約ワークフローを実行してください。

1. `20_Literature` フォルダに配置された Markdown 形式の論文を読み込みます。
2. 内容を要約してください（日本語、300〜500 文字）。
3. 要約を `summaries/同名ファイル-summary.md` として保存してください。

## 🧾 フォーマット例（出力）

```markdown
---
source: papers/example_paper.md
summary-date: 2025-06-15
---

### 要約

この研究は、〜〜〜〜に関するものであり、主な目的は〜〜〜〜である。著者らは〜〜を用いて〜〜を検証し、結果として〜〜を発見した。これは〜〜という意味を持ち、今後の〜〜に影響を与える可能性がある。
```
