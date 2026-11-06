# 理解の過程と表現の選び直し

[索引へ](00_index.md) · [書誌一覧](07_sources_and_search_log.md)

## P01 Russell et al. (1993)

**The Cost Structure of Sensemaking** — Daniel M. Russell, Mark J. Stefik, Peter Pirolli, Stuart K. Card. CHI '93, 誌面pp.269–276。[DOI](https://doi.org/10.1145/169059.169209)／[著者公開PDF](https://www.markstefik.com/wp-content/uploads/2014/04/1993-Cost-Structure-of-Sensemaking1.pdf)。

### 原典から得る点

[原典の整理] 表現の探索、情報の符号化、表現の変更を繰り返す。既存の表現に収まりにくい情報や欠けた情報を含む「residue」が変更の契機となる。検索だけ速くしても、理解に必要な作業全体のコストが下がるとは限らない。プリンター技術者の教材設計の事例を通じて議論する。[原文、Abstract、ケーススタディ、Learning Loops、PDF pp.1–3](https://www.markstefik.com/wp-content/uploads/2014/04/1993-Cost-Structure-of-Sensemaking1.pdf)。

### 今回への適用

[応用案] 文章・比較表・局所的な関係図を切り替えられるようにする。「分類不能」「この説明では扱えない」結果を残し、情報側を削る前に分類や表現を見直す。理解しやすさはノード数や圧縮率だけでは評価しない。

**限界**：この事例とコストの議論は、現代の解析レポートにおける最適UIや、特定のグラフ形式の優位性を決めるものではない。

**採用判断**：表現形式を設計する際の補助文献。活動全体の入口はP02を先に読む。

## P02 Pirolli & Card (2005)

**The Sensemaking Process and Leverage Points for Analyst Technology as Identified Through Cognitive Task Analysis** — Peter Pirolli, Stuart Card. International Conference on Intelligence Analysis。[公開PDFのミラー](https://andymatuschak.org/files/papers/Pirolli%2C%20Card%20-%202005%20-%20The%20sensemaking%20process%20and%20leverage%20points%20for%20analyst%20technology%20as.pdf)。DOIは今回確認できていない。

### 原典から得る点

[原典の整理] 情報を探し選び抽出するforaging loopと、証拠を構造化して仮説・成果物を作るsensemaking loopを区別する。原資料、収集資料、抜き出した証拠、schema、仮説、提示物を扱い、証拠からの構築と仮説からの再探索を往復する。情報分析者の認知的課題分析に基づく暫定的なモデルである。[原文§2.2、Figure 2、PDF pp.2–4](https://andymatuschak.org/files/papers/Pirolli%2C%20Card%20-%202005%20-%20The%20sensemaking%20process%20and%20leverage%20points%20for%20analyst%20technology%20as.pdf)。

### 今回への適用

[応用案] 「結果収集→要約→終了」と固定せず、仮説の比較で不足が見つかれば元の図表や追加解析へ戻る。少なくとも、元資料への入口、根拠の整理、解釈の比較、提示物の編集を別の作業として確認する。

**限界**：情報分析者の活動の記述であり、全領域に適した固定工程や品質保証手順ではない。原典自身が一般化に注意を求める（Introduction）。LLMの内的認知モデルとして扱わない。

**採用判断**：最初に読む。今回の仕組みで支援する活動と、戻れる経路を決めるための入口とする。

## P05 Sacha et al. (2014)

**Knowledge Generation Model for Visual Analytics** — Dominik Sacha, Andreas Stoffel, Florian Stoffel, Bum Chul Kwon, Geoffrey Ellis, Daniel A. Keim. IEEE TVCG 20(12), 誌面pp.1604–1613。[DOI](https://doi.org/10.1109/TVCG.2014.2346481)／[研究グループ公開PDF](https://bib.dbvis.de/uploadedFiles/article_final.pdf)。

### 原典から得る点

[原典の整理] 人間と計算側をつなぐexploration、verification、knowledge generationのループを示す。Findingは分析中の興味深い観察であり、対象領域の文脈で解釈されてInsightにつながる。Findingが必ずInsightになるわけではない。既存のVisual Analyticsシステムへのモデルの対応づけも示す。[原文Figure 1、§2.2–2.4、§4](https://bib.dbvis.de/uploadedFiles/article_final.pdf)。

### 今回への適用

[応用案] 「群Aの指標が高い」という観察、「機序Xが影響した」という仮説、追加確認を通じた理解を区別して保存する。仮説から「次にどの結果を確認すれば区別できるか」を作業に落とす。

**限界**：概念モデルとその利用例が中心であり、Insightを自動判定する学習済み分類器や、妥当性の保証ではない。ここで提案するObservation・Hypothesisの保存形式を原典の仕様と同一視しない。

**採用判断**：P02と活動上の重なりはあるが、用語と情報オブジェクトを設計する際に追加する価値がある。

## 3本を組み合わせる際の境界

[調査に基づく判断] P02で作業の往復を、P01で表現変更を、P05で観察と解釈の関係を考える。3本の図を一つの厳密な状態遷移図へ無理に統合しない。人間の理解の変化と、システムが保存できる情報は別である。
