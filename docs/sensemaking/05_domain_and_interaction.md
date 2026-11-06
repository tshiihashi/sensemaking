# 領域の作業と対話的な探索

[索引へ](00_index.md) · [書誌一覧](07_sources_and_search_log.md)

## P09 Mirel & Görg (2014)

**Scientists’ Sense Making When Hypothesizing About Disease Mechanisms from Expression Data and Their Needs for Visualization Support** — Barbara Mirel, Carsten Görg. BMC Bioinformatics 15, Article 117。[DOI](https://doi.org/10.1186/1471-2105-15-117)／[出版社の全文](https://link.springer.com/article/10.1186/1471-2105-15-117)／[PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC4021544/)。出版社の掲載区分はCommentary。

[原典の実証結果] 発現データから疾患機序を考える研究者1名を6か月調査した。可視化の操作だけでなく文献読解、外在化、仮説と執筆を含む流れを記述する。ただし重要な合成・Insightの生起をすべて直接観察したわけではない。[原文Methods、Descriptions of sense making stages、Limitations and future directions](https://link.springer.com/article/10.1186/1471-2105-15-117)。

[原典の整理] 複数ツールの間でデータを移すこと、メモや図解を利用すること、データと文献を関連づけることを支援する設計指針を提案する。[原文Guidelines for tool design](https://link.springer.com/article/10.1186/1471-2105-15-117)。

**適用条件と限界**：オミクス解析を想定するなら直接性が高い。単一ケースの探索的知見であり、研究者一般の時間配分や最適手順として一般化しない。

[応用案] 遺伝子・経路の一致だけで機序の主張を統合しない。試料、細胞種、比較、解析条件、参照文献を保持し、他ツールへの出力と再読可能なメモを支える。今回の対象が生物学と確定していないため、一般設計の必須前提にはしない。

**採用判断**：生物学で試行する場合に読む。実際の作業が単一ツールで閉じない点を確認する。

## P10 Endert et al. (2012)

**Semantic Interaction for Sensemaking: Inferring Analytical Reasoning for Model Steering** — Alex Endert, Patrick Fiaux, Chris North. IEEE TVCG 18(12), 誌面pp.2879–2888。[DOI](https://doi.org/10.1109/TVCG.2012.260)／[著者要旨を掲載したIEEE VIS公式ページ](https://ieeevis.org/year/2012/paper-session/all/all)／[PubMed書誌](https://pubmed.ncbi.nlm.nih.gov/26357197/)。

**確認範囲**：公式会議ページの要旨と書誌を確認。本文・評価節は未確認。

[原典の整理：要旨] ForceSPIREで、文書の移動、強調、検索などの操作をキーワード重みの調整に結びつけ、利用者とともに空間配置を作るsemantic interactionを扱う。利用者調査を報告している。[IEEE VIS公式ページ、該当タイトルのAbstract](https://ieeevis.org/year/2012/paper-session/all/all)。

**適用条件と限界**：操作とモデルのパラメータを対応づけられる探索に参考となる。参加者数、課題、比較条件、効果量は今回未照合。LLMによる根拠判定や知識の真偽を検証した研究ではない。

[応用案] AIが関連候補を提案し、人間の選択や修正を探索順位に反映する方向は検討できる。ただし「近くに移動した」ことを「支持した」と自動解釈しない。操作の意味と、明示的な論証関係を分ける。

**採用判断**：AIと人間の対話設計を具体化する段階で本文を追加確認する。現段階では着想源に限定する。

## P11 Stasko et al. (2008・Jigsaw)

**Jigsaw: Supporting Investigative Analysis through Interactive Visualization** — John Stasko, Carsten Görg, Zhicheng Liu. Information Visualization 7(2), 誌面pp.118–132。[DOI](https://doi.org/10.1057/palgrave.ivs.9500180)／[著者公開PDF](https://faculty.cc.gatech.edu/~stasko/papers/iv08-jigsaw.pdf)。関連するVAST 2007論文の拡張版として参照する。

[原典の整理] 文書中の人物・組織・場所などのエンティティを複数の連動ビューで探索する。同じ文書に登場することが関係探索の重要な入口となる。[原文Analyzing documents、System description、PDF pp.2–8](https://faculty.cc.gatech.edu/~stasko/papers/iv08-jigsaw.pdf)。

[原典の整理] 論文末尾では、探索の出発点がない状態からの全体概観に弱く、いくつかの対象エンティティがある場合に有用と述べる。VASTコンテストでの利用経験はあるが、専門分析者による評価は今後の課題としている。[原文Discussion and future work、PDF p.12](https://faculty.cc.gatech.edu/~stasko/papers/iv08-jigsaw.pdf)。

**適用条件と限界**：多数文書にまたがる対象の接続をたどる用途に向く。共起は支持・反証や因果を表さない。この2008年版の記述を現行ツールの機能一覧として扱わない。

[応用案] 共通対象からレポートを探す入口は用意するが、その後に比較条件と主張の内容を確認する。初期画面には検索だけでなく、論点・対象・未確認範囲の一覧など別の入口も比較する。

**採用判断**：横断探索のUIを検討するときに読む。知見の保存モデルをこれだけで決定しない。

## 使い分け

[調査に基づく判断] P09は領域の実際の作業、P10は操作と計算モデルの接続、P11は文書横断の探索を補う。いずれも、主張の根拠・競合・更新を管理する情報構造を単独で完成させる文献ではない。[構造の文献](03_claims_evidence_and_synthesis.md)と併せて検討する。
