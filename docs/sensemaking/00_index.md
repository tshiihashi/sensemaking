# Sensemakingシステムのための文献調査

調査日：2026-11-06（日本時間）。対象は、複数の解析結果・主張・根拠・解釈を関連づけ、理解の形成と更新を支援する仕組みである。出発点は[データ解析レポートの4課題](../../data_analysis_reporting_challenges.md)。

## 今回の答え

[調査に基づく判断] **主張と根拠の関係を保存するだけでなく、その関係や表現を後から修正できることが重要である。** 設計候補としては、原資料への参照を保つノートから始め、必要な部分を観察・仮説・関係へ段階的に構造化し、読者には目的に合う表や文章を提示する構成を推す。[文献選定](01_scope_and_reading_plan.md)と[方式比較・具体案](06_design_comparison.md)に判断の根拠を示す。

これは論文群から導いた応用案であり、実装・利用者評価を済ませた標準手順ではない。グラフの優位性を一律に主張する根拠も得られていない。

## 構成と読み順

| 資料 | 内容 |
| --- | --- |
| [01_scope_and_reading_plan.md](01_scope_and_reading_plan.md) | 採否の基準、13本の優先順位、重複と相補性、当初の紹介文の補正 |
| [02_process_and_representation.md](02_process_and_representation.md) | Russell、Pirolli & Card、Sacha：表現の変更、探索・仮説検討、知見形成 |
| [03_claims_evidence_and_synthesis.md](03_claims_evidence_and_synthesis.md) | Uren、Waldner、Chan：主張単位の構造、原資料との接続、研究ノートへの導入 |
| [04_ambiguity_formalization_and_provenance.md](04_ambiguity_formalization_and_provenance.md) | Shipman & Marshall、Nowak & Bartram、Xu、Dung：形式化の負担、曖昧さ、来歴、競合する論証 |
| [05_domain_and_interaction.md](05_domain_and_interaction.md) | Mirel & Görg、Endert、Jigsaw：生物学の分析、操作からのモデル調整、文書横断探索 |
| [06_design_comparison.md](06_design_comparison.md) | 実装方式の比較、最小の情報構造、手順、架空例、評価方法 |
| [07_sources_and_search_log.md](07_sources_and_search_log.md) | 全論文の書誌・DOI・公開原文、アクセス状況、検索方法、未確認範囲 |

まず01で読む対象を選び、06で今回の課題との対応を把握する。個別の設計判断に必要な論文だけ02〜05へ戻る。

## 原典と応用の区別

- `[原典の整理]`：当該論文の説明・主張。
- `[原典の実証結果]`：当該論文が実施した観察・実験の結果。対象と条件を併記する。
- `[応用案]` / `[調査に基づく判断]`：本リポジトリ向けの提案・選定判断。
- `[架空例による確認]`：説明用の例についての整合確認。実データでの有効性検証ではない。

PDFの `PDF p.` は**先頭ページを1**とする。誌面のページを使う場合は「誌面」と明記する。HTMLは節名で示す。本文の関連節を確認したものは11本、要旨・公開紹介に確認範囲を限定したものはUrenとEndertの2本である。確認状況の詳細は07を参照。

## 既存資料との関係

[Visualization InsightのSoK整理](../systemization_of_knowledge/00_index.md)は、知見の発見・保管・伝達を結ぶ全体像を扱う。今回はその内容を置き換えず、個別原著を確認して「関係の表現」「構造化の負担」「解釈の更新」を補う。[既存のAgent向け設計](../systemization_of_knowledge/05_agent_reporting_design.md)と[テンプレート](../systemization_of_knowledge/06_templates_and_checklists.md)も引き続き応用案として扱う。

## 調査の範囲と残る不確実性

これは提示された文献を起点とする目的別調査であり、体系的レビューでも2026年までの網羅的な最新動向調査でもない。13本を整理し、追加候補としてChanらのDiscourse Graph研究とDungの論証理論を採用した。リポジトリ名の空き状況、現行製品の比較、アプリやskillの実装は対象外とした。

未完了なのは、Uren・Endertの評価方法の本文照合、LLMによる関係提案の精度評価、実際の解析成果物を使った方式比較である。文献が得た人間向けの結果を、そのままAgentの性能保証として用いない。

## 生物学・創薬への追加調査

[創薬・バイオインフォマティクス研究におけるSensemaking](../biomedical_sensemaking/00_index.md)では、生物ネットワーク・生物医学データ・化学空間・不確実性のレビュー4本と、MirelらやWGS解釈の実証研究3本を整理し、原典PDFを保存した。今回のP09を含むが、領域全体を単独で網羅するSensemakingレビューとは区別している。

## レポートを読む人への補完調査

[読者の理解・納得感・認知負荷](../reader_understanding/00_index.md)では、完成した文章・図表を読む人の理解、説明や引用への依存、根拠を検証する手間を補った。本調査の分析者向けの知識整理と組み合わせるための編集・評価案を含む。日本語の実レポートでの利用者評価は未実施。
