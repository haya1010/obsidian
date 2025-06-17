---
title: 論文要約タスクの順次実行
description: 未実施の論文について、各種要約とリンク付与を順番に実行するためのテンプレート
tags: [summary, sequential-tasks, cursor-workflow]
---

## 📂 対象論文ファイルのパス

[`summaries/papers/論文ファイル名.md`](../summaries/papers/論文ファイル名.md)

## 📌 タスク

以下の順序で要約タスクを実行してください：

1. 驚き屋風ストーリー型要約の作成
2. Figure ごとの実験内容と結果の要約の作成
3. Figure ごとの要約（パネル説明を含む）の作成
4. 元論文への要約リンクの付与

## 🧾 実行手順

### 1. 驚き屋風ストーリー型要約の作成

1. [`templates/story_style_summary_request.md`](../templates/story_style_summary_request.md) の指示内容を確認し、忠実に実行してください。
2. 特に以下の点に注意：
   - 5 章構成（🕰 ～ 🌐）に従って記述
   - 科学的な正確性とストーリー性の両立
   - 出力先の確認

### 2. Figure ごとの実験内容と結果の要約の作成

1. [`templates/figure_summary_template.md`](../templates/figure_summary_template.md) の指示内容を確認し、忠実に実行してください。
2. 特に以下の点に注意：
   - 各 Figure の 4 項目（目的・手法・結果・解釈）の記述
   - 画像の適切な配置
   - 出力先の確認

### 3. Figure ごとの要約（パネル説明を含む）の作成

1. [`templates/fig_summary_template.md`](../templates/fig_summary_template.md) の指示内容を確認し、忠実に実行してください。
2. 特に以下の点に注意：
   - 各 Figure 内のパネル（a, b, c...）の役割を文中に盛り込む
   - 4 項目を 1 つの Figure 単位で記述
   - 画像の適切な配置
   - 出力先の確認

### 4. 元論文への要約リンクの付与

1. [`templates/add_summary_links_template.md`](../templates/add_summary_links_template.md) の指示内容を確認し、忠実に実行してください。
2. 特に以下の点に注意：
   - YAML frontmatter の直後の配置
   - リンクセクションの形式
   - ファイル名のエンコード

## 📝 注意事項

1. 各要約は、前の要約が完了してから次の要約を開始してください。
2. 各要約ファイルの存在を確認してから、元論文へのリンクを追加してください。
3. ファイル名のエンコードを忘れずに行ってください。
4. 各要約の内容は、元論文の内容と整合性が取れていることを確認してください。

## 🔄 実行順序の理由

1. ストーリー型要約を最初に作成することで、論文全体の流れを把握
2. 実験内容と結果の要約で、各 Figure の詳細な分析
3. パネル説明を含む要約で、Figure 内の各パネルの役割を明確化
4. 最後に元論文へのリンクを追加して、各種要約へのアクセスを容易に
