# 生物学のSensemakingを直接扱う実証研究

[索引](00_index.md) · [レビュー](01_review_papers.md) · [統合整理](03_synthesis_and_research_log.md)

この3本は包括的なレビューではない。レビューだけでは分かりにくい「研究者が何をしているのか」を補う。ページ番号は保存PDFの先頭を1とする。

## E1 Mirel & Görg (2014)：発現データから疾患機序の仮説へ

**Barbara Mirel, Carsten Görg.** *Scientists’ sense making when hypothesizing about disease mechanisms from expression data and their needs for visualization support*. BMC Bioinformatics **15**, 117, 2014。掲載区分：Commentary。[DOI・全文](https://doi.org/10.1186/1471-2105-15-117)／[保存PDF](../../papers/biomedical_sensemaking/Mirel_Gorg_2014_Scientists_Sense_Making.pdf)。[既存の短い整理](../sensemaking/05_domain_and_interaction.md#p09-mirel--görg-2014)に対して、今回はPDF保存と関連節の確認を追加した。

[原典の実証結果：Methods、PDF pp.10–11] 心不全の治療非応答に関する仮説を作る研究者1名を6か月調査した。可視化操作の記録、インタビュー、研究ノート等から過程を再構成する。創薬の標的探索・疾患機序理解に近いが、新薬開発プロジェクト全体の調査ではない。

[原典の整理：Descriptions of sense making stages、pp.3–9、Figures 1, 3–8] 研究目的に基づく6段階を提案する。

1. 遺伝子の機能属性を整理し、探索対象を絞る。
2. 関連する遺伝子を経路・生物学的事象へ位置づけ、説明の候補を得る。
3. 文献を読んで背景と生物学的なストーリーを理解する。
4. 文献のMethods・Results等を詳しく読み、どうして起こるのかを説明する。
5. 図式化して条件・機序を明確にし、仮説を作る。
6. 論文・提案書の執筆のために文献と根拠を再読する。

直線的な手順ではなく、矛盾・根拠不足があれば前段へ戻るモデルである。複数ツール、文献、ノートや因果図の間の移動が重要になる。

[原典の整理：Guidelines for tool design、pp.8–10] 選択的な絞り込みと拡張、データ交換、柔軟なレイアウト、異なる関係・視点の比較、知識の外在化、文献の発見・注釈、調査履歴の保存を提案する。

**限界。** 1ケースを一般的な研究者の標準工程・時間配分へ一般化できない。著者はStages 3–4の重要な合成・Insightを直接観察していないことを認め、協働も十分には対象にしていない（Limitations、p.10）。

[応用案] Agentの成果物を遺伝子リストや経路図で止めず、どの実験条件・文献を使ってどの説明へ進んだかを記録する。説明が整ったことと、機序が実証されたことを区別する。

**採用判断：今回のSensemakingという問いに最も直接的。** 認知過程を理解する中心文献としてR1と併読する。

## E2 Mirel (2009)：分類できても説明できない問題

**Barbara Mirel.** *Supporting cognition in systems biology analysis: findings on users’ processes and design implications*. Journal of Biomedical Discovery and Collaboration **4**, 2, 2009。[DOI・全文](https://doi.org/10.1186/1747-5333-4-2)／[保存PDF](../../papers/biomedical_sensemaking/Mirel_2009_Supporting_Cognition.pdf)。

[原典の実証結果：Abstract、Results、Methods、PDF pp.1, 4–10, 13–14] 生物医学研究者15名がMiMIとMiMI–Cytoscapeを用いてタンパク質相互作用から疾患機序を探索する作業を観察・インタビューした。観察回数は参加者間で異なり、全員を同じ期間・回数追跡した比較試験ではない。

[原典の整理：Review of relevant research / Discussion、pp.2–3, 10–13] 属性・パターンを読み取るclassification、条件や機序を考えるmodel-based reasoning、因果関係を説明するnarrative reasoningを区別する。結果の読み取りを支える機能が、そのまま深い説明の形成を支えるとは限らない。

[原典の実証結果：Discussion、pp.11–13] 主要な不一致は、①データ・ツール・解釈の妥当性を確認すること、②分類からモデルに基づく推論へ移ること、③因果的なmental modelを組み立てること。出典や実験の種類、関係の条件、表示を組み替える柔軟性が重要になる。

**限界。** 当時の特定ツールと探索課題に基づく。2026年のCytoscapeや現在のAgentが同じ問題を持つと、そのまま断定できない。相互作用の発見から因果説明への飛躍を問題化する概念的な土台として使う。

[応用案] 「同じ経路に属する」「発現が相関する」「直接結合する」「介入で変化する」を別の証拠として保存する。Agentが関係を統合する際には、関係の種類とその出典を明示する。

**採用判断：E1の前提を深める。** 有意差・クラスタ・関連候補の大量出力だけでは、なぜ現象が起こるかの説明にならない理由を考えるときに読む。

## E3 Mastrianni et al. (2024公開版／2025出版)：AI支援と再解釈

**Angela Mastrianni, Hope Twede, Aleksandra Sarcevic, Jeremiah Wander, Christina Austin-Tse, Scott Saponas, Heidi Rehm, Ashley Mae Conard, Amanda K. Hall.** *AI-Enhanced Sensemaking: Exploring the Design of a Generative AI-Based Assistant to Support Genetic Professionals*。

- 保存・本文確認：arXiv:2412.15444v1、2024-12-19。[arXiv](https://arxiv.org/abs/2412.15444)／[DOI](https://doi.org/10.48550/arXiv.2412.15444)／[保存PDF・28ページ](../../papers/biomedical_sensemaking/Mastrianni_2024_AI_Enhanced_Sensemaking_arxiv_v1.pdf)。
- 後続出版：ACM Transactions on Interactive Intelligent Systems、2025。[出版DOI](https://doi.org/10.1145/3756326)。出版の存在は確認したが、出版版PDFは未取得、保存版との全文差分は未照合。以下は保存版の内容である。

[原典の実証結果：§4–6、PDF pp.7–17] 希少疾患のWGS解釈に関わる専門家17名へのインタビューと、専門家6名との共同設計等を実施する。文献・データベース・症例情報の収集と統合、他者への共有、再解析する症例の優先づけを扱う。

[原典の整理：§7.2–7.3、pp.18–21] AIが文献の情報をまとめ、遺伝子・変異の表など更新可能な成果物を作り、専門家が確認・修正する設計を検討する。共有される解釈、初回の理解と新証拠による再解釈、複数の情報様式の統合を設計上の論点とする。

**限界。** 共同設計とプロトタイプへのフィードバックであり、AIによる診断率向上・見逃し低減・作業時間短縮を比較試験で実証した研究ではない。設計段階の参加者が同一機関であることと、自発参加による選択の偏りを述べる。タスクに基づく利用者試験は今後の課題とされる（§7.4–8、p.22）。

[応用案] 知見保管庫に、出典、AIが作成した部分、人間の訂正、確認状態、更新によって再検討すべき主張を持たせる。他者の確認を一括した「正しい」というラベルへ置き換えず、何を確認したかを残す。

**採用判断：Agent向けの設計に近い補助文献。** WGSという限定された作業から得た設計上の知見であり、創薬全般の自動化性能の根拠にはしない。
