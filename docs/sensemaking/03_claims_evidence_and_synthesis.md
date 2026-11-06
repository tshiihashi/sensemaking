# 主張・根拠・原資料をつなぐ構造

[索引へ](00_index.md) · [書誌とアクセス状況](07_sources_and_search_log.md)

## P03 Uren et al. (2006)

**Sensemaking Tools for Understanding Research Literatures: Design, Implementation and User Evaluation** — Victoria Uren, Simon Buckingham Shum, Michelle Bachler, Gangmin Li. IJHCS 64(5), 誌面pp.420–445。[DOI](https://doi.org/10.1016/j.ijhcs.2005.09.004)／[研究機関の公開説明](https://kmi.open.ac.uk/publications/techreport/kmi-05-09)／[公開原稿PDF](https://kmi.open.ac.uk/publications/pdf/KMI-TR-05-9.pdf)。

**確認範囲**：出版社の検索表示、研究機関の要旨と原稿冒頭の検索表示を確認。PDFはWeb取得時にサイズ制限となり、本文・評価節は未確認。公開説明は2005年の技術報告、上の書誌は2006年の掲載論文を指す。

### 原典から確認できた点

[原典の整理：要旨] 研究者が文献の貢献と他文献との概念的関係を主張として表す仕組みを扱う。ClaiMapperはargument mapの作成、ClaiMakerは保存と文献横断の問い合わせ、ClaimFinderは検索サービスへの入口を担う。[研究機関の要旨](https://kmi.open.ac.uk/publications/techreport/kmi-05-09)。

### 今回への適用

[応用案] 文書へのタグだけでなく、「誰が、どの主張を、どの根拠から関連づけたか」を残す。同じ文書を読んだ人が異なる関係を提案する場合も、関係の作成者と理由を分けて保存する。

**限界・保留**：正確な関係型の一覧、評価対象・人数、効果量、使い勝手の問題は本文未照合であり転記しない。自動的に科学的正しさを判定するシステムと解釈しない。

**採用判断**：主張単位の設計に直接関係するため優先する。ただし実装スキーマをそのまま採用する判断は保留する。

## P04 Waldner et al. (2021)

**Linking Unstructured Evidence to Structured Observations** — Manuela Waldner, Thomas Geymayer, Dieter Schmalstieg, Michael Sedlmair. Information Visualization 20(1), 誌面pp.47–65。[DOI](https://doi.org/10.1177/1473871620986249)／[著者所属機関公開PDF](https://www.cg.tuwien.ac.at/research/publications/2021/waldner-2021-leo/waldner-2021-leo-Paper.pdf)。

### 原典から得る点

[原典の整理] Flexible observation graphと文書中の根拠箇所を双方向のdeep linkで接続する。観察だけでなく関係にも根拠を付けられ、元の文書を再表示できる。[原文Table 1、設計節、PDF pp.5–6](https://www.cg.tuwien.ac.at/research/publications/2021/waldner-2021-leo/waldner-2021-leo-Paper.pdf)。

[原典の実証結果] 学術環境のknowledge worker 20名を2群に分け、大画面・1時間の文書分析でテキストエディタと比較した。グラフ群は同時に開いておく文書ウィンドウが少なかった。一方、真相を発見する能力への効果は証拠不足としている。[原文Participants、Results、PDF pp.8–11](https://www.cg.tuwien.ac.at/research/publications/2021/waldner-2021-leo/waldner-2021-leo-Paper.pdf)。

### 今回への適用

[応用案] 「出典URL」だけでなく、ファイル版・ページ・節・表の行など確認先の位置を保存する。観察から元の図表へ戻る経路と、元の図表から利用中の主張を探す経路を用意する。

**限界**：大画面の短時間実験を、そのまま長期的な科学分析や一般的な小画面UIに適用できない。文書との接続があることと、主張の正しさが検証されることも異なる。

**採用判断**：原資料を残したまま構造化する接続方法として優先する。グラフ表示の採用は別に評価する。

## P12 Chan et al. (2024・追加)

**Steps Towards an Infrastructure for Scholarly Synthesis** — Joel Chan, Matthew Akamatsu, David Vargas, Lukas Kawerau, Michael Gartner。[arXiv:2407.20666v2](https://arxiv.org/abs/2407.20666v2)／[本文HTML](https://arxiv.org/html/2407.20666v2)。今回はプレプリントv2として参照し、査読済み掲載版は確認していない。

### 原典から得る点

[原典の整理] Question・Claim・Evidenceを扱うDiscourse Graphを、ハイパーテキストの研究ノートへ組み込む。非形式的なノートと形式的な要素を併存させ、段階的な構造化を支援する。[原文§4](https://arxiv.org/html/2407.20666v2#S4)。

[原典の実証結果] 約2.5年の展開を含むResearch through Design。48名との直接的な接触・観察、41件の調査回答、5名の半構造化インタビュー等を用いる。ノード作成の導入可能性を示す一方、関係を滑らかに記述する負担が残った。[原文§3、§5–6.1](https://arxiv.org/html/2407.20666v2#S3)。

### 今回への適用

[応用案] 全解析結果に最初から厳密な型を要求せず、普段のメモのうち繰り返し使う部分を昇格させる。関係を作る作業には「どの問いに答えるためか」という即時の便益を付ける。

**限界**：利用者コミュニティでの質的研究であり、無作為化比較による一般的な生産性向上の証明ではない。48・41・5は別の情報源の人数で、合算しない。論文当時の拡張機能の記述を、現在の製品仕様として案内しない。

**採用判断**：今回追加した中で最も直接性が高い。入力の継続性と、知識構造の維持負担を検討するために読む。

## 3本を比較した設計上の含意

[調査に基づく判断]

| 設計上の問い | 主な参照 | この調査での判断 |
| --- | --- | --- |
| 文書を超えた理解を何として保存するか | P03、P12 | 主張・根拠・問いを識別する。ただし型の細部は固定しすぎない |
| 保存内容をどこまで検証できるか | P04 | 元資料の具体箇所へ戻れる参照を持つ |
| 関係は事実か、利用者の判断か | P03、P04 | 関係そのものにも理由・根拠・作成者を持たせる |
| 続けて入力してもらえるか | P12 | 後の共有だけでなく、今の比較・執筆に役立つ入口を作る |

3本が共通の正解スキーマを実証したわけではない。とくにUrenの正確な型と評価は未確認であり、上表は各研究から導いた設計判断である。
