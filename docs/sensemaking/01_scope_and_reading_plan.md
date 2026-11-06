# 文献の選定と読む順番

[索引へ](00_index.md) · [出典と確認状況](07_sources_and_search_log.md)

## 1. 何を調べるか

入力は複数の解析結果、図表、レポート、研究ノートを想定する。利用者はそれらを比較して説明を考える分析者と、その根拠を確認したい読者である。人数、成果物数、対象領域は未指定なので、特定のDB・UI・LLMを前提にしない。

[調査に基づく判断] [既存の4課題](../../data_analysis_reporting_challenges.md)を次の設計上の問いに分けた。

| 課題 | 文献から確かめること |
| --- | --- |
| 注目した現象以外を見逃す | 仮説に合わない結果から探索・表現を見直せるか |
| 網羅すると情報過多になる | 原資料の保持と、読者への提示を別に設計できるか |
| 分散した結果の関係が分からない | 文書単位を超えて、主張・観察と出典を接続できるか |
| 複数の妥当な解釈がある | 競合、条件、保留、変更の履歴を表現できるか |

採用基準は、これらの問いへの直接性、他論文では補えない役割、一次情報の確認可能性とした。被引用数や発表年だけで優先順位を決めていない。

## 2. 選定した13本

以下の順位は今回の構想に対する判断であり、学術的な重要度のランキングではない。各行の詳細と根拠はリンク先にある。

| ID | 論文 | 優先度 | 読む目的 |
| --- | --- | --- | --- |
| P01 | Russell et al. (1993) | 理論の補足 | 表現を選び直すコストを考える → [02](02_process_and_representation.md#p01-russell-et-al-1993) |
| P02 | Pirolli & Card (2005) | 優先1 | 探索から仮説・報告へ往復する全体像 → [02](02_process_and_representation.md#p02-pirolli--card-2005) |
| P03 | Uren et al. (2006) | 優先2 | 文献の主張と議論関係を扱う先行設計 → [03](03_claims_evidence_and_synthesis.md#p03-uren-et-al-2006) |
| P04 | Waldner et al. (2021) | 優先3 | 原資料の具体箇所と構造化した観察を接続 → [03](03_claims_evidence_and_synthesis.md#p04-waldner-et-al-2021) |
| P05 | Sacha et al. (2014) | 理論の補足 | Finding・Hypothesis・Insightの区別 → [02](02_process_and_representation.md#p05-sacha-et-al-2014) |
| P06 | Nowak & Bartram (2024) | 優先5 | 曖昧さを残す表示と比較の条件 → [04](04_ambiguity_formalization_and_provenance.md#p06-nowak--bartram-2024) |
| P07 | Xu et al. (2015) | 優先7 | 来歴の記録・表示・再利用 → [04](04_ambiguity_formalization_and_provenance.md#p07-xu-et-al-2015) |
| P08 | Shipman & Marshall (1999) | 優先4 | 早すぎる形式化と入力負担を避ける → [04](04_ambiguity_formalization_and_provenance.md#p08-shipman--marshall-1999) |
| P09 | Mirel & Görg (2014) | 用途別 | 生物学での実際の作業の流れを確認 → [05](05_domain_and_interaction.md#p09-mirel--görg-2014) |
| P10 | Endert et al. (2012) | 用途別 | 人間の操作とモデルの調整をつなぐ → [05](05_domain_and_interaction.md#p10-endert-et-al-2012) |
| P11 | Stasko et al. (2008) | 用途別 | 文書を横断する探索のUI → [05](05_domain_and_interaction.md#p11-stasko-et-al-2008jigsaw) |
| P12 | Chan et al. (2024) | 優先6・追加 | 研究ノートから主張・根拠の構造を育てる → [03](03_claims_evidence_and_synthesis.md#p12-chan-et-al-2024追加) |
| P13 | Dung (1995) | 用途別・追加 | 競合する論証の受容を形式的に考える → [04](04_ambiguity_formalization_and_provenance.md#p13-dung-1995追加) |

**最小の5本はP02 → P03 → P04 → P08 → P06。** 全体像、主張の表現、出典への接続、形式化の負担、複数解釈の保持を一巡できる。P03は公開要旨までの確認なので、具体的なスキーマ採用前には本文の追加確認が必要である。運用まで考えるとP12とP07を続ける。

## 3. 追加した理由と、後回しにしたもの

[調査に基づく判断]

- **P12を追加**：UrenとWaldnerに加え、主張・根拠の構造を日常の研究ノートで継続して作れるかを検討できる。技術構造だけでなく、導入と保守の問題に答える。
- **P13を追加**：競合を記録することと、一定の規則で受容する論証集合を計算することを区別できる。初期実装に論証ソルバーを要求するための選定ではない。
- **P01・P05は補足**：P02で活動の全体像を押さえた後、表現形式や用語を具体化する段階で読む。
- **書籍とObsidianは保留**：今回の一次論文調査では、機能の代替性や製品選定まで広げない。Kleinの書籍を読了した根拠として引用していない。
- **一般的なKnowledge Graph・RAG研究は今回は保留**：保存・検索技術だけでは、条件つきの主張、競合、構造化の負担に答えたことにならない。自動抽出・検索を実装する段階で別途調べる。

## 4. 重複は何を意味するか

| 組み合わせ | 共通点 | 代替できない部分 | 読み分け |
| --- | --- | --- | --- |
| Russell／Pirolli & Card | 理解と表現の反復 | 表現のコスト／分析活動の全体像 | 最初は後者、表現の設計時に前者 |
| Pirolli & Card／Sacha | 探索・仮説検討の反復 | 分析作業の流れ／人間と計算の接続・知見形成 | 用語・オブジェクト設計に後者を追加 |
| Uren／Waldner | 文書を超えた関係づけ | 主張の議論関係／原資料と観察の相互参照 | 同じ「グラフ」として一本化しない |
| Uren／Chan | 主張・根拠を扱う構造 | 先行システム／日常のノートへの導入過程 | 導入負担は後者で補う |
| Shipman／Chan | 段階的な形式化 | 形式化に伴う問題の整理／研究ノートでの具体化 | 原則と実例として併読 |
| Nowak／Dung | 競合を扱う | 人間の解釈が複数ある状態／攻撃関係が与えられた論証の意味論 | 不確実性の数値化とは分ける |
| Pirolli & Card／Xu | 分析過程 | 活動のモデル／過程を記録して使う課題 | 来歴は独立に設計する |

この表は論文群を比較した本資料の整理であり、重複率の計測や研究の発展史を示すものではない。

## 5. 提示された紹介文から補正すべき点

1. **P05の主要語はFinding。** 本資料のObservationやData factと対応づけるのは設計上の選択であり、原典が同じスキーマを規定したとは扱わない。[P05の原文§2](https://bib.dbvis.de/uploadedFiles/article_final.pdf)。
2. **P04は一般的な精度向上の証明ではない。** 原典は課題の真相発見への効果を結論できないと述べる。[P04の原文、PDF p.10](https://www.cg.tuwien.ac.at/research/publications/2021/waldner-2021-leo/waldner-2021-leo-Paper.pdf)。
3. **曖昧さと統計的不確実性を一括りにしない。** P06が扱う複数解釈は、誤差棒や信頼区間を追加するだけで解決するとはいえない。[P06の原文§1](https://ieeevis.b-cdn.net/vis_2023/pdfs/v-full-1573.pdf)。
4. **文書の共起、主張への支持、因果関係を分ける。** Jigsawをそのまま主張の妥当性評価に置き換えない。[P11の原文「Analyzing documents」](https://faculty.cc.gatech.edu/~stasko/papers/iv08-jigsaw.pdf)。
5. **Compression／Synthesis／Sensemakingは今回の作業上の区別。** 三者を排他的な標準分類としては引用しない。要約が統合や理解を助ける場合もある。今回の目標は「新しい関係・問い・解釈を検討できること」に置く。
