# 創薬・バイオインフォマティクス研究におけるSensemakingの文献調査

調査日：2026-11-06（日本時間）。[リポジトリの課題](../../data_analysis_reporting_challenges.md)と[一般的なSensemakingの調査](../sensemaking/00_index.md)を、生物学・創薬の研究場面へ具体化するための追加調査。

## 回答と対象範囲

**関連する包括的な論文はある。まずEhlersら（2025）の生物ネットワーク可視化サーベイを推す。** 複数のデータ源、ネットワーク解析、可視化、操作、仮説探索をつなぎ、不確実性・条件間比較・来歴を未解決課題として整理している。[R1・原典](https://doi.org/10.1016/j.cag.2024.104115)

ただし、**創薬研究とバイオインフォ研究のSensemaking全般を、研究者の認知・文献読解・仮説改訂・共同作業・報告まで単独で網羅するレビューは、今回の探索では確認できなかった。** 「存在しない」という結論ではない。包括的な可視化レビュー4本と、Sensemakingを直接調べた実証研究3本を組み合わせる。化学空間の図示と、疾患機序の説明形成は関連するが、同一の作業とは扱わない。

ここでのSensemakingは、解析結果を既存知識や文献と関連づけ、仮説や説明を作り、根拠に戻って更新する研究活動を指す。科学教育、組織アイデンティティ、臨床診療全般のSensemakingは中心対象から外した。WGS研究はバイオインフォの解釈作業に近い補助事例として含める。

## 保存した7本と読む順番

PDFはすべて[専用ディレクトリ](../../papers/biomedical_sensemaking/README.md)に保存済み。ページ数は**保存したPDFの先頭を1とする総ページ数**。Rはレビュー／サーベイ、Eは実証研究。優先順位は今回の課題に基づく判断であり、引用数ランキングではない。

| 優先 | ID・論文 | 種別・範囲 | 今回読む理由 | PDF |
| --- | --- | --- | --- | --- |
| 1 | R1 Ehlers et al. (2025), *An introduction to and survey of biological network visualization* | 生物ネットワークの83論文を整理 | データ・解析・表現・操作を横断する入口 | [31ページ](../../papers/biomedical_sensemaking/Ehlers_2025_Biological_Network_Visualization.pdf) |
| 2 | E1 Mirel & Görg (2014), *Scientists’ sense making when hypothesizing about disease mechanisms from expression data and their needs for visualization support* | 研究者1名・6か月のケース研究。掲載区分はCommentary | 発現解析から文献読解・機序仮説・執筆への実際の往復 | [12ページ](../../papers/biomedical_sensemaking/Mirel_Gorg_2014_Scientists_Sense_Making.pdf) |
| 3 | R2 O’Donoghue et al. (2018), *Visualization of Biomedical Data* | 生物医学の広いレビュー | 情報過多を避ける表現と、探索・伝達の設計 | [30ページ](../../papers/biomedical_sensemaking/ODonoghue_2018_Visualization_of_Biomedical_Data.pdf) |
| 4 | R3 AlShammari et al. (2026), *Chemical space visualization at scale: a survey of end-to-end pipelines and dataset-size archetypes* | 化学空間の56研究を整理 | 創薬の化合物集合・構造活性関係・大規模探索 | [37ページ](../../papers/biomedical_sensemaking/AlShammari_2026_Chemical_Space_Visualization.pdf) |
| 5 | R4 Weiskopf (2022), *Uncertainty Visualization: Concepts, Methods, and Applications in Biological Data Visualization* | 不確実性の概念レビュー | 観測・変換・表現から生じる不確実性の保持 | [17ページ](../../papers/biomedical_sensemaking/Weiskopf_2022_Uncertainty_Visualization.pdf) |
| 6 | E2 Mirel (2009), *Supporting cognition in systems biology analysis: findings on users’ processes and design implications* | 研究者15名のフィールド研究 | パターンの分類から機序の説明へ進む際の難しさ | [17ページ](../../papers/biomedical_sensemaking/Mirel_2009_Supporting_Cognition.pdf) |
| 7 | E3 Mastrianni et al., *AI-Enhanced Sensemaking: Exploring the Design of a Generative AI-Based Assistant to Support Genetic Professionals* | WGS専門家へのインタビュー・共同設計 | AI生成の知識表、共有、再解釈を考える | [2024年arXiv v1・28ページ](../../papers/biomedical_sensemaking/Mastrianni_2024_AI_Enhanced_Sensemaking_arxiv_v1.pdf) |

E3には2025年の査読済み出版がある（[DOI: 10.1145/3756326](https://doi.org/10.1145/3756326)）。**今回保存・本文確認したのは2024年のarXiv v1であり、出版版との全文差分は未照合。** Ehlers論文は2024年オンライン公開・2025年巻号掲載のため、ここでは2025年と表記する。

## 資料構成

| 資料 | 内容 |
| --- | --- |
| [01_review_papers.md](01_review_papers.md) | レビュー4本の書誌、対象範囲、主要な整理、適用条件と限界 |
| [02_empirical_studies.md](02_empirical_studies.md) | 実証研究3本の研究条件、Sensemaking過程、設計への示唆 |
| [03_synthesis_and_research_log.md](03_synthesis_and_research_log.md) | 4課題との対応、方式比較、試行手順、架空例、検索・取得記録、追加候補 |
| [PDF一覧と取得情報](../../papers/biomedical_sensemaking/README.md) | 正式タイトル、取得元、版、ページ数、保存状況 |

バイオインフォの機序解釈なら **R1 → E1 → E2**、創薬の化合物探索なら **R3 → R4 → R2**、Agentの知見管理なら **E1 → E3 → 統合整理** の順が適している。

## 確認範囲と区別

- `[原典の整理]`：当該論文の説明・主張。レビューが分類する個別手法の性能は、原著を独立に再検証したものではない。
- `[原典の実証結果]`：当該研究自身の観察・インタビュー等で得られた結果。
- `[応用案]` / `[調査に基づく判断]`：このリポジトリ向けの提案。実データやAgentで有効性を検証した結果ではない。

7本のPDFについて読み込み、ページ数、先頭の書誌、本文の関連節を確認した。全引用文献の原著照合・全ツールの現行機能確認・完全なシステマティックレビューは行っていない。未取得の関連2本と検索上の限界は[調査記録](03_synthesis_and_research_log.md#検索と取得の記録)に明記する。
