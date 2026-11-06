# 文章理解と情報提示：読者に何が伝わるか

[索引](00_index.md) · [信頼と検証](02_trust_and_verification.md) · [設計案](03_report_design.md)

以下は完成した文章・図表を読む場面を中心に選んだ一次研究である。PDFページは先頭を1とする。書誌・版・取得状態は[出典一覧](05_sources_and_search_log.md)にまとめる。

## A1 August et al. (2024)：平易さと情報量と読者の知識を分ける

*Know Your Audience: The benefits and pitfalls of generating plain language summaries beyond the “general” audience.* [DOI](https://doi.org/10.1145/3613904.3642289)／[保存PDF](../../papers/reader_understanding/August_2024_Know_Your_Audience.pdf)。

[原典の実証結果：§4〜6] 3つの参加者内研究（N=199、191、203）で、人またはLMによる科学要約の複雑さと読者の話題への馴染みを調べた。低い馴染みの読者は平易な要約の読書体験を高く評価した。一方、馴染みのある読者は、平易すぎる要約の折り畳み節を開かない傾向があり、限界の説明も対象となった。情報を削らず説明すると、平易な版は長くなった。

**適用と限界。** 米国の英語母語話者を中心とするオンライン研究。主な評価は読書体験の自己申告、折り畳み節のクリック記録、原文への関心であり、客観的な理解テストの向上と読み替えない。開いた節を熟読したかも分からない。馴染みは専門資格と同一ではない。

[応用案] 読者の知識・目的・時間を入力に加える。平易化の際は「用語を説明した」のか「情報を落とした」のかを確認し、重要な限定条件を残す。全読者に最短の同一要約を出す設計の根拠にはしない。

## A2 Markowitz (2024)：分かったという感想と実際の理解を照合する

*From complexity to clarity: How AI enhances perceptions of scientists and the public’s understanding of science.* [DOI](https://doi.org/10.1093/pnasnexus/pgae387)／[掲載版HTML](https://pmc.ncbi.nlm.nih.gov/articles/PMC11406778/)。

[原典の実証結果：Study 2、Study 3、Table 1] 米国の参加者に、同じ科学論文のGPTによる平易な要約とPNAS掲載要約を提示した（Study 2: N=274、Study 3: N=250）。Study 3の理解の合成指標と自由記述の採点はGPT版で高かったが、選択式問題単独の差は有意ではなかった。信頼性の評価が高まる効果も両研究で一様ではない。

**適用と限界。** 刺激は言語差の大きな要約対から選ばれ、自由記述はLLMで採点された。文章の平易さ以外も異なるため、「短文なら理解が上がる」「AIなら人よりよい」と一般化しない。長い解析レポートや日本語の検証ではない。

[応用案] 読みやすさの感想に加えて、読者自身の言葉で主張と条件を説明してもらう。自由記述の判定をAgentだけで完結させない。

## A3 Chandler & Sweller (1992)：理解に必要な情報を離しすぎない

*The split-attention effect as a factor in the design of instruction.* [DOI](https://doi.org/10.1111/j.2044-8279.1992.tb01017.x)／[保存PDF](../../papers/reader_understanding/Chandler_Sweller_1992_Split_Attention.pdf)。

[原典の実証結果：Experiment 2、PDF pp.7〜10] 教育心理学の学生20名に、実験報告の通常構成と、対応する手続・結果等をまとめた構成を無作為に割り当てた。統合した版は処理時間が短く、質問への得点が高かったと報告する。認知負荷そのものの直接測定は限定的で、時間を間接指標としている。

**適用と限界。** 初学者と比較的単純な報告の研究である。著者も、専門家・複雑な報告では異なる可能性、通常の節構成が再読・検索を助ける利点を挙げる。結果の直後へ方法全文を複製する指示にはしない。

[応用案] 各主要結果の近くに、理解に必要な母数・比較条件・集計単位だけを置く。詳細な方法は参照先に残し、往復しないと意味が取れない状態を減らす。

## A4 Zhi, Ottley & Metoyer (2019)：文章と図の配置・リンクを評価する

*Linking and Layout: Exploring the Integration of Text and Visualization in Storytelling.* [DOI](https://doi.org/10.1111/cgf.13719)／[原著者公開PDF](https://visualdata.wustl.edu/files/linking.pdf)。

[原典の整理：著者要旨] 180名のクラウドソーシング研究で、縦配置とスライドショー形式、文章と図の対話的なリンクを比較し、関与・理解・再生を測定した。従来のSoK整理で既に紹介されていた研究を、今回の読者側の論点へ接続する。

**確認範囲は著者要旨と書誌のみ。** Web経由のPDF読取は容量制限、直接取得はタイムアウトとなり、今回本文・結果節を独立に確認できていない。配置名を単純な「縦対横」に置き換えると表示方式の違いが落ちる。静的Markdownと対話的ストーリーを同一条件とみなさない。本調査では具体的な優劣の採用根拠にしない。

[応用案] まず図番号・対象条件・該当箇所を文章で指し示す。対話的リンクや横並びの採用は、画面幅と読者課題を揃えて別に比較する。

## A5 Shao et al. (2024)：単一の要点と複数の知見では効果を分ける

*Data Storytelling in Data Visualisation: Does it Enhance the Efficiency and Effectiveness of Information Retrieval and Insights Comprehension?* [DOI](https://doi.org/10.1145/3613904.3643022)／[確認したarXiv v2本文](https://arxiv.org/html/2402.12634v2)／[保存PDF](../../papers/reader_understanding/Shao_2024_Data_Storytelling_arxiv_v2.pdf)。

[原典の実証結果：§3、§4.2〜4.4] 103名が通常の可視化とストーリー要素を加えた可視化を読み、情報検索と知見理解の問題に答えた。全課題の正答率は後者で高かったが、全体の所要時間には有意差がなかった。単一知見の理解では時間短縮が報告された。複数知見・情報検索の時間へ同じ効果を広げない。

**適用と限界。** 強調・注釈・タイトル等をまとめて変更しており、各要素の独立効果は分からない。v2の§4.4には検定結果と周辺の要約文が一致しない箇所があるため、詳細の課題別検定を優先した。競合する因果仮説を含む長い報告は対象外。

[応用案] 主論点の説明に注釈を使いつつ、横断的な比較には共通条件の表を用意する。注釈を足せば「すべての読者・課題で速くなる」とは扱わない。

## この5本からの採用判断

[調査に基づく判断] 文章の平易化は、情報の削減と分離して行う。主要な結果は、その意味を取るのに必要な条件や図表と対応付ける。ただし、読書体験、正答率、時間、記憶は別の結果であり、どれか一つの改善を他へ転用しない。日本語の語彙や文長の閾値は、今回の英語研究から定めない。
