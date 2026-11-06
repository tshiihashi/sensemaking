# 包括的なレビュー・サーベイ4本

[索引](00_index.md) · [実証研究](02_empirical_studies.md) · [比較と調査記録](03_synthesis_and_research_log.md)

ページ番号は、リンク先の保存PDFの先頭を1とする。章・節名も併記する。レビューが紹介する個別研究の効果は、この調査で独立に検証した結果ではない。

## R1 Ehlers et al. (2025)：生物ネットワークを横断する入口

**Henry Ehlers, Nicolas Brich, Michael Krone, Martin Nöllenburg, Jiacheng Yu, Hiroaki Natsukawa, Xiaoru Yuan, Hsiang-Yun Wu.** *An introduction to and survey of biological network visualization*. Computers & Graphics **126**, 104115, 2025。オンライン公開：2024-11-23。[DOI](https://doi.org/10.1016/j.cag.2024.104115)／[著者側の紹介](https://www.cg.tuwien.ac.at/research/publications/2025/ehlers-2025-ait/)／[保存PDF](../../papers/biomedical_sensemaking/Ehlers_2025_Biological_Network_Visualization.pdf)。

**包括性とSensemakingとの距離。** キーワードにSensemaking loopを含むが、論文の分類枠はCardらのInformation Visualization Pipelineである。Sensemakingの認知理論の総説というより、生物ネットワークを理解・探索するための技術と作業の総覧として読む。

[原典の整理：§2、PDF pp.2–4、Figures 1–2] グラフモデル、グラフ解析、ネットワーク表現、解析課題、対話操作、応用分野の6要素で全体を整理する。700本超の初期検索と手動追加・選別を経て83本を採用し、比較図ではグラフ解析・表現・課題・応用分野の4軸へ分類する。遺伝子制御、タンパク質相互作用、代謝、multi-omics、ゲノム変異、系統などを扱う（§8、pp.18–22）。

[原典の整理：§9–10、pp.23–25] 研究課題は、①模式図・直線node-link図以外の表現、②不確実性、③高度なグラフ解析との統合、④条件・試料・時点間の比較、⑤来歴と信頼、⑥動的ネットワークの6点。特に、ネットワークの存在する辺をすべて同じ確実さで描くことや、密な全体図で読者を圧倒する問題が重要になる。

**適用条件と限界。** 生物学的な関係をネットワークに表せる解析に向く。コミュニティ検出やスケーラビリティの網羅的整理などは対象外・不足と著者自身が認める。6分類を整備すれば研究者の仮説形成が改善する、と実験的に保証する論文ではない。

[応用案] 知見同士を一枚の大きなグラフへ集める前に、「対象を比較する」「経路をたどる」「条件ごとの違いを見る」などの問いを決め、表・局所ネットワーク・階層を使い分ける。生物学的相互作用のネットワークと、主張を支持・反証する論証のネットワークは区別する。

**採用判断：最初に読むレビュー。** 本リポジトリの「分散する結果の関係」「情報過多」「条件依存」の3点に特に近い。

## R2 O’Donoghue et al. (2018)：探索と伝達の広いレビュー

**Seán I. O’Donoghue, Benedetta Frida Baldi, Susan J. Clark, Aaron E. Darling, James M. Hogan, Sandeep Kaur, Lena Maier-Hein, Davis J. McCarthy, William J. Moore, Esther Stenau, Jason R. Swedlow, Jenny Vuong, James B. Procter.** *Visualization of Biomedical Data*. Annual Review of Biomedical Data Science **1**, 誌面pp.275–304, 2018。[DOI・出版社](https://doi.org/10.1146/annurev-biodatasci-080917-013424)／[保存PDF](../../papers/biomedical_sensemaking/ODonoghue_2018_Visualization_of_Biomedical_Data.pdf)。保存版は大学リポジトリ公開のReview in Advance体裁である。

[原典の整理：Data Integration and Tailored Visualizations、PDF p.7] 有用な可視化には、対象現象の理解に必要な複雑さを選ぶこと、解釈に必要な文脈を加えること、それらを一貫した表現へ統合することが必要だと論じる。情報を単に減らすだけではなく、何を理解するための表示かが選択基準になる。

[原典の整理：Visualization for Discovery / Communication / Perspectives、pp.7–23] ゲノム、single-cell RNA-seq、構造生物学、systems biology、画像・組織、メタゲノム等を横断する。概要から詳細への移動、連動する複数ビュー、クラスタリングなどを共通戦略として挙げる。Systems Biology（pp.15–17）では、force-directed図が密になる問題を指摘する。

**適用条件と限界。** 広い分野の可視化方針と科学的伝達を考える入口。Sensemakingの全工程や複数仮説の保存形式を体系化したレビューではない。2018年のツール・構造情報の充足状況などを現在の仕様や統計として流用しない。

[応用案] 保管庫には結果と条件を保持し、読者向け表示では「主要な現象・解釈に必要な文脈・結論を変え得る例外」を先に示す。除外した結果にも戻れるようリンクする。この保存方式は本資料の提案である。

**採用判断：表示とレポートを設計するときに読む。** R1より生物医学全般を広く扱うが、研究者が説明を形成する実際の作業はE1・E2で補う。

## R3 AlShammari et al. (2026)：創薬に近い化学空間探索

**Maha M. AlShammari, Moayad Alnammi, Moataz Ahmed.** *Chemical space visualization at scale: a survey of end-to-end pipelines and dataset-size archetypes*. Journal of Cheminformatics **18**, 112, 2026。公開：2026-06-02。[DOI・出版社](https://doi.org/10.1186/s13321-026-01223-4)／[保存PDF](../../papers/biomedical_sensemaking/AlShammari_2026_Chemical_Space_Visualization.pdf)。

[原典の整理：Review methodology、PDF pp.2–4、Table 2] 56研究を、データセット、分子特徴量、次元削減、クラスタリング、評価の5段階で比較する。要旨は対象期間を2000–2025年と記す一方、Search strategyでは2000年から2025年初めまでとする。2025年末まで網羅したレビューとは表記しない。

[原典の整理：Abstract、Gaps and future research directions / Conclusion、pp.1, 31–32] データ規模に応じた工程の組み合わせを提案する。大きい集合を処理できることと、化学的関係を正しく保つことの両方が必要で、見た目や一般的な埋め込み評価だけでは不足する。構造類似性、scaffold、近傍保持、前処理・パラメータの再現可能な記録を重視する。

**適用条件と限界。** 化合物ライブラリの多様性、構造活性関係、候補領域の探索に直接役立つ。創薬全体のSensemaking、標的機序の文献統合、チームの意思決定を網羅しない。主に明示的に列挙された分子集合が対象であり、組合せ規則だけで表現する巨大空間は同じ条件で扱えない。レビューの工程例は、全条件で比較実験済みの最適手順ではない。

[応用案] 「2次元図で離れているから機序が違う」とは判断しない。特徴量・距離・次元削減の設定を保存し、元の化学的類似性と活性測定条件へ戻る。候補領域、外れ値、activity cliffを別々の検討対象として保持する。

**採用判断：創薬の化合物探索では最優先。** 生物学的な説明・標的妥当性の判断にはE1・E2などが別に必要になる。

## R4 Weiskopf (2022)：不確実性を落とさないためのレビュー

**Daniel Weiskopf.** *Uncertainty Visualization: Concepts, Methods, and Applications in Biological Data Visualization*. Frontiers in Bioinformatics **2**, 793819, 2022。[DOI・出版社](https://doi.org/10.3389/fbinf.2022.793819)／[保存PDF](../../papers/biomedical_sensemaking/Weiskopf_2022_Uncertainty_Visualization.pdf)。

[原典の整理：§1, §3、PDF pp.1–6] 不確実性は入力データだけでなく、フィルタ、変換、可視化、知覚・認知、対話操作を通じても生じ、伝播する。著者は、全手法を網羅するsystematic surveyではなく、概念・原則・方針を広くカバーするレビューだと明記する。

[原典の整理：§4–6、pp.7–15] 分布の明示、サンプルによる暗示、区間や統計量、視覚属性、複合表示を整理し、グラフを例に説明する。実務上は対象とタスクを定め、不確実性の主要な発生源を優先し、表示領域・読み取りの難しさ・実装負担を考慮する。

**適用条件と限界。** 測定値や推定・ネットワーク関係の確かさを表示する設計に向く。主として確率的にモデル化できる不確実性を扱う。競合する生物学的説明や「測定していない」「文献が不足している」といった状態を、すべて単一の誤差棒や確率に還元できるわけではない。

[応用案] 保存項目を「測定誤差」「解析条件による差」「既知関係の根拠」「解釈の競合」「未確認」に分け、意味の異なる不確実性を混ぜない。本文には判断を変える不確実性を優先表示し、詳細へ戻れるようにする。

**採用判断：R1・R3を補う共通の基盤。** 不確実性をすべて図に載せれば理解しやすくなる、という保証として使わない。
