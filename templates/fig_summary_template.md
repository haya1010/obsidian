---
title: Figure ごとの要約（パネル説明を含む）
description: Figure 1, 2... 単位でまとめ、その中に含まれる(a), (b), (c)...のパネルを自然な流れで記述してください。
tags: [summary, figure, cursor-workflow]
---

## 📂 対象論文ファイルのパス

[`summaries/papers/論文ファイル名.md`](../summaries/papers/論文ファイル名.md)

---

## 📌 タスク

1. 各 Figure（例：Figure 1, Figure 2）に対応する説明文を読み取ってください。
2. 以下の 4 項目を**1 つの Figure 単位で**記述しつつ、その中に含まれる各パネル（a, b, c など）がどのような役割を果たしているかを文中に盛り込んでください：
   - 実験の目的
   - 使用した手法
   - 得られた主な結果（パネルに対応づけて）
   - 結果の解釈・意義
3. 画像（Markdown 形式の `![](https...)`）がある場合は、その Figure 内で適切な位置にそのままコピーしてください。
4. 出力は `summaries/fig_summaries/論文ファイル名_fig_summary.md` に保存してください。
5. 出力内のファイルリンク（例：`[元論文を開く](../papers/論文ファイル名.md)`）は、  
   **スペースを `%20` に変換したエンコード形式**で記述してください。

例：  
`A vagus nerve dominant tetra-synaptic ascending pathway.md`  
→ `A%20vagus%20nerve%20dominant%20tetra-synaptic%20ascending%20pathway.md`

---

## 🧾 出力フォーマット例

```markdown
---
source: 20_Literature/論文ファイル名.md
summary-date: 2025-06-15
type: figure_summary
---

> 🗂 [元論文を開く](../papers/論文ファイル名.md)

## Figure 1

この図では、○○ 処理が体重や代謝に与える影響を評価している。

(a) では、実験スケジュールと介入プロトコルが示されている。  
(b) は処理群と対照群の体重推移をタイムコースで比較したもので、処理群では 3 日目以降に体重減少が顕著に現れた。  
(c) は (b) のデータを定量化した結果で、有意差（p < 0.01）が確認されている。

![](https://example.com/fig1.png)

---

## Figure 2

この図は、処理後の行動変化を測定したものである。

(a) に示されるように、実験動物は処理後に活動量が低下し、(b) のグラフでは群間差が定量的に示されている。  
(c) ではオープンフィールドでの移動距離が可視化されており、結果は処理の影響を支持する内容であった。
(d) に示すように VMHBDNF ニューロンに GCamp を発現させ、(e)に示すようなカルシウム応答が見られた。

![](https://example.com/fig2.png)
```
