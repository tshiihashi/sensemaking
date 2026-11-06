# 曖昧さ、形式化の負担、来歴、競合する論証

[索引へ](00_index.md) · [書誌と確認状況](07_sources_and_search_log.md)

## P08 Shipman & Marshall (1999)

**Formality Considered Harmful: Experiences, Emerging Themes, and Directions on the Use of Formal Representations in Interactive Systems** — Frank M. Shipman III, Catherine C. Marshall. CSCW 8, 誌面pp.333–352。[DOI](https://doi.org/10.1023/A:1008716330212)／[大学公開PDF](https://ics.uci.edu/~corps/phaseii/ShipmanMarshall-FormalityConsideredHarmful-JCSCW.pdf)。

[原典の整理] 問題として認知的負担、暗黙知、早すぎる構造の強制、状況によって変わる構造を挙げる。対処には段階的・システム支援による形式化などがある。形式化そのものを廃止する主張ではなく、利用者の目的・状況に必要な明示化の水準を合わせる議論である。[原文§3–4、PDF pp.8–17](https://ics.uci.edu/~corps/phaseii/ShipmanMarshall-FormalityConsideredHarmful-JCSCW.pdf)。

**適用条件と限界**：初期の曖昧な探索や、型の選択が負担になる状況で重要。複数システムの経験を基にした議論であり、形式化の費用を普遍的に数値化した実験ではない。

[応用案] 初回の記録には本文と出典を優先し、未分類のメモを許す。関係を「関連あり・理由未整理」として置いた後、必要なものを支持・反対・条件依存へ具体化する。AIの型づけも候補として戻せるようにする。

**採用判断**：グラフを中心とする設計を決める前に読む。ノード・エッジの豊富さを、そのまま使いやすさとみなさないための文献とする。

## P06 Nowak & Bartram (2024)

**Designing for Ambiguity in Visual Analytics: Lessons from Risk Assessment and Prediction** — Stan Nowak, Lyn Bartram. IEEE TVCG 30(1), 誌面pp.924–933。[DOI](https://doi.org/10.1109/TVCG.2023.3326571)／[IEEE VIS公開PDF](https://ieeevis.b-cdn.net/vis_2023/pdfs/v-full-1573.pdf)。会議の公開原稿は2023年、巻号年は2024年。

[原典の整理] Ambiguityを、複数の解釈がもっともらしい、あるいは望ましい状態として扱う。[原文§1、PDF p.1](https://ieeevis.b-cdn.net/vis_2023/pdfs/v-full-1573.pdf)。

[原典の実証結果] 雪崩予報者10名が過去データによる2シナリオを、既存の表中心の道具とAvObsで評価した。現在の状況を判断するnowcast課題であり、将来予測の精度試験ではない。結果は概ね似ていたが解釈活動に違いがあり、どちらかが総合的に優れるとは結論していない。[原文§5–6、PDF pp.4–8](https://ieeevis.b-cdn.net/vis_2023/pdfs/v-full-1573.pdf)。

**適用条件と限界**：文脈や細部で解釈が変わる領域に示唆がある。専門家の既存ツールへの習熟、領域・標本数、模擬課題の条件があり、一般的なUI原則の全面否定とは読まない。

[応用案] 要約から元資料へ戻るだけでなく、必要な細部を並べたまま異なる仮説を比較できる表示も用意する。確率の低さ、データの欠損、解釈の競合を一つの「確信度」に畳み込まない。

**採用判断**：複数解釈を保持する設計に必須。要約と詳細の切り替えだけで十分かを問い直す。

## P07 Xu et al. (2015)

**Analytic Provenance for Sensemaking: A Research Agenda** — Kai Xu, Simon Attfield, T. J. Jankun-Kelly, Ashley Wheat, Phong H. Nguyen, Nallini Selvaraj. IEEE CG&A 35(3), 誌面pp.56–64。[DOI](https://doi.org/10.1109/MCG.2015.50)／[機関リポジトリ](https://openaccess.city.ac.uk/id/eprint/15535/)／[受理原稿PDF](https://openaccess.city.ac.uk/id/eprint/15535/1/CG_CG%26ASI-2014-12-0110.R1_Xu.pdf)。

[原典の整理] 来歴をevent、action、sub-task、taskの階層で捉える。低水準の操作記録と高水準の目的は異なり、後者を操作から推定することには限界がある。記録・可視化・利用、協働、不確実性と信頼などの研究課題を整理する。[原文§1–5、受理原稿のPDF pp.3–12](https://openaccess.city.ac.uk/id/eprint/15535/1/CG_CG%26ASI-2014-12-0110.R1_Xu.pdf)。

**適用条件と限界**：後日の検証、引き継ぎ、解釈の見直しで重要。研究アジェンダであり、来歴を残せば誤りを防げるという効果検証ではない。

[応用案] データ版、解析条件、使った根拠、採用・保留・改訂の理由を成果物として残す。記録対象は検証可能な判断と操作の結果であり、Agentの非公開の内部思考を逐語的に保存することを要件にしない。

**採用判断**：後からEvidenceを追加・訂正する構想では早い段階で読む。完全な操作ログより、再確認に必要な情報を先に定める。

## P13 Dung (1995・追加)

**On the Acceptability of Arguments and its Fundamental Role in Nonmonotonic Reasoning, Logic Programming and n-Person Games** — Phan Minh Dung. Artificial Intelligence 77(2), 誌面pp.321–357。[DOI](https://doi.org/10.1016/0004-3702(94)00041-X)／[大学公開PDF](https://cse-robotics.engr.tamu.edu/dshell/cs631/papers/dung95acceptability.pdf)。

[原典の整理] 論証集合と二項のattack関係からなる抽象的枠組みを定義し、競合しない集合、受容可能性、preferred・stable・grounded等の意味論を扱う。複数の受容集合が成立する場合がある。基本枠組みでは論証の内部構造を抽象化する。[原文§2.1–2.2、PDF pp.5–10](https://cse-robotics.engr.tamu.edu/dshell/cs631/papers/dung95acceptability.pdf)。

**適用条件と限界**：attack関係と採用する意味論を明示できる場合の基礎理論。支持の重み、統計的不確実性、根拠の独立性、自然言語からのattack抽出は、この基本モデルだけで解決しない。人間向けUIの有効性実験でもない。

[応用案] 「関係として記録されている」と「ある規則で受容された」を別フィールドにする。後者を計算するなら意味論も保存する。初期段階では、競合を一覧できる表と変更履歴で足りるかを先に検討する。

**採用判断**：形式的な結論候補の計算が必要になった場合に追加する。支持・反対のラベルを付けただけの知見グラフを、Dungの論証枠組みと同一視しない。

## 区別して保持したいもの

以下は原典の共通分類ではなく、今回の情報構造への提案である。

| 状態・情報 | 保存する内容 | 混同を避ける点 |
| --- | --- | --- |
| 統計的な不確実性 | 推定量、区間、方法、対象集団 | 数値の変動と解釈の違いは別 |
| 情報の不足・出典の問題 | 未測定、欠損、未確認、資料版 | 「測定されなかった」と「効果がなかった」は別 |
| 解釈の曖昧さ | 成立し得る説明、文脈、比較すべき細部 | 単一の確信度で解消したことにしない |
| 見かけの不一致 | 対象・期間・定義・集計単位の違い | 条件をそろえる前に反証と断定しない |
| 論証間の競合 | 何に対して、なぜ反対するか | 共起や語の類似度をattackとしない |
| 判断の変更 | 旧判断、新判断、変更の根拠と影響先 | 新しい版が旧主張を「反証」するとは限らない |

P08が記述の負担、P06が人間の解釈、P07が記録と再利用、P13が形式的な受容規則を扱う。これらを一つの「不確実性対応機能」で済ませない。
