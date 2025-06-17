---
title: 実験事実抽出ログ
description: 指定された論文.mdをもとに、各段落やFigureから得られた観察事実のみを淡々と抽出します。
tags: [fact-extraction, experiment-log, data-centric, cursor-workflow]
---

## 📂 対象論文ファイルのパス

`papers/論文ファイル名.md`

---

## 📌 タスク

以下のルールに従って、論文の本文および Figure の説明から**客観的な実験事実**のみを抽出・列挙してください：

1. 主観的解釈・仮説・目的・考察は含めず、**「何が起きたのか」だけ**を書く。
2. 各事実は 1 行ずつの箇条書き形式で記載。
3. 対応する Figure やパネル (a), (b)... があればそのラベルも明記。
4. 単なる "増加した" や "変化した" ではなく、「どの群で」「何が」「どのように」変化したか、**定量的な記述**を心がける。
5. 出力ファイルは `summaries/fact_extractions/論文ファイル名_fact_extraction.md` に保存してください。

---

## 🧾 出力フォーマット（コピーして使用）

```markdown
---
source: papers/論文ファイル名.md
summary-date: 2025-06-15
type: fact_extraction
---

## 実験事実の記録

- Figure 1a: GD 処理群では、NTS 領域の c-Fos 陽性細胞数が対照群の 2.5 倍に増加した。
- Figure 1b: Vagotomy 後、GD による NTS の c-Fos 活性化は消失した。
- Figure 2c: LPB におけるチャネルロドプシン導入後の光刺激により、PL 皮質での EPSC が誘発された。
- Paragraph 4: PVT へのウイルス注入により、LPB → PVT 投射が可視化された。
- Figure 4a: GD 刺激によって PL 皮質でのカルシウムシグナルが急激に上昇した（ΔF/F > 0.3）。
- Figure 5: NTS–LPB–PVT–PL の順伝播回路を光操作で遮断すると、GD 誘発行動が顕著に減弱した。

...
```
