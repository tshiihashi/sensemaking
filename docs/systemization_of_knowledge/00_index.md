# Visualization Insight 論文の詳細整理とAgentレポート作成への応用

## この資料の目的

`Systemization_of_Knowledge.pdf` の内容を日本語で整理し、Agentによるデータ解析レポート作成スキルを設計する際の参照資料として保存する。論文の要約と、そこから導いた設計案を分ける。今回は参照資料を作成しており、実行可能なスキルの作成・インストールは行っていない。

原典：Chen He, Niklas Elmqvist, Andrea Bellucci, Mahdi Munshi, Giulio Jacucci. *Systemization of Knowledge (SoK): Visualization Insight – Two Decades of Research, Practice, and Future Directions*. ACM Computing Surveys 58(9), Article 224, February 2026, 37 pages. DOI: 10.1145/3788869。

- [原典PDF](../../papers/Systemization_of_Knowledge.pdf)
- [このリポジトリの既存の課題整理](../../data_analysis_reporting_challenges.md)
- 以下の `p.` / `pp.` はPDFの先頭を1とするページ。誌面の `224:3` はPDFのp.3に対応する。
- `[原典の整理]` は論文の説明・著者の主張、`[レビュー対象研究の報告]` は論文が紹介する個別研究の結果、`[応用案]` は本資料で追加したAgent向けの設計である。
- 個別研究はこのPDFによる二次的な整理に基づく。原著論文の実験条件や実装を独立に確認したものではない。

## ファイル構成と読み方

| ファイル | 主な内容 | 用途 |
|---|---|---|
| [01_overview_and_model.md](01_overview_and_model.md) | 問題設定、レビュー手法、用語、Figure 1の循環モデル、既存モデルとの関係 | 全体像と設計の土台を理解する |
| [02_theory_and_empirical_findings.md](02_theory_and_empirical_findings.md) | 理論2領域・実証5領域、評価、外在化、バイアス、結果の解釈上の制限 | 何を知見として扱い、どう評価するかを決める |
| [03_technologies_and_systems.md](03_technologies_and_systems.md) | 技術9領域、知見管理、グラフ、ファクト採掘、レポート生成、ML/LLM | 保存形式・生成方式・システム構成を検討する |
| [04_future_directions_and_limits.md](04_future_directions_and_limits.md) | 5つの研究方向、論文の限界、Agentに転用する際の注意 | 未解決問題と適用範囲を把握する |
| [05_agent_reporting_design.md](05_agent_reporting_design.md) | 既存課題との対応、Agentの手順、採用判断、スキル分割案、評価 | スキル仕様のたたき台にする |
| [06_templates_and_checklists.md](06_templates_and_checklists.md) | 知見・仮説・関係・来歴のテンプレート、レポート雛形、レビュー項目 | 後の実装に再利用する |

まず01でモデルを理解し、05で実務への対応を読む。スキルを具体化する際は06を使い、判断根拠が必要になった部分だけ02〜04へ戻る。

## 論文の核心

[原典の整理：pp.2–4, 22–28]

1. **Insightは数値や図そのものではなく、理解・知識の前進である。** データ上の傾向を抽出することと、対象領域を理解することは区別される。
2. **データファクトを対象領域の情報と結び付ける必要がある。** 文脈を欠いた自動生成結果は、適用可能性や行動へのつながりが弱い。
3. **発見・記録・整理・伝達は循環する。** レポート作成は解析終了後の一方向の工程ではなく、新しい問いや再検証を生む。
4. **知見とデータ・図・注釈・分析来歴の接続が重要である。** 後から検証、再利用、引き継ぎができる形で外在化する。
5. **自動化には質の保証が必要である。** 多重比較、認知バイアス、誤解を招く図、ドメイン情報の不足が知見の有効性を損なう。

## 今回の課題に対する中心的な示唆

[応用案]

「すべてを一つの長いレポートに書く」ことと「一つの筋書きに絞る」ことの間に、**知見保管庫を持ち、その一部を目的別・階層別にレポート化する**設計を置く。

- 保管庫には、採用した知見だけでなく、反証、例外、複数の解釈、保留結果を、根拠とともに残す。
- 本文には、読者の問いに関係する知見と、判断を変え得る条件・反証を選ぶ。
- 詳細や未採用結果にはリンクで到達できるようにする。
- 書いている途中に根拠不足や矛盾が分かれば、解析へ戻る。

この構成は論文のモデルや紹介事例に着想を得た提案であり、論文がそのままAgent用の標準手順として検証したものではない。

## 原典の章と参照先

| 原典 | PDFページ | この資料 |
|---|---:|---|
| Abstract / 1 Introduction | 1–3 | 01 |
| 2 Background | 3–4 | 01 |
| 3 Method and Analysis | 4–7 | 01、04 |
| 4.1 Theoretical Research | 7–9 | 02 |
| 4.2 Empirical Studies | 9–13 | 02 |
| 4.3 Technological Research | 13–23 | 03 |
| 5 Modeling the Cycles of Visualization Insight | 23–24 | 01 |
| 6 Discussion and Future Research Directions | 24–28 | 04 |
| 7 Conclusion | 28 | 00、04 |
| References | 28–35 | 02〜04の研究名・原典内文献番号 |
| Appendix A–D | 36–37 | 01、04 |

参考文献158件の全件解説や原文翻訳は含めず、本文の16研究トピックと5つの将来方向を整理した。具体的なフィールド名、状態名、品質チェック、レポート雛形は本資料の提案である。

## 関連する追加調査

[Agentの作業・保存ファイルの統合案](../agent_workflow/01_workflow_and_files.md)では、本資料と追加調査を踏まえ、各stepの記録、知見、横断比較、図、1つのレポートをつなぐ汎用的な運用を提案する。ファイル別の保存項目、更新時期、最小構成、雛形を含む。実データでの有効性は未検証。

[Sensemakingシステムのための文献調査](../sensemaking/00_index.md)では、主張・根拠の関係、原資料への接続、段階的な形式化、曖昧さ、分析来歴を扱う13本を別途整理した。個別原著の確認範囲と未確認事項は同資料に示す。本ディレクトリ全体の引用を原著照合済みへ変更したものではない。

[レポート読者の理解・納得感・認知負荷の補完調査](../reader_understanding/00_index.md)では、科学要約の平易化、予備知識、図表との対応、説明・出典・不確実性と信頼、負荷の測定を扱う。既存の階層的レポート案を読者側から補い、編集手順と読者評価案を示す。応用案の利用者試験は未実施である。
