# Mechanisms of Action (MoA) Prediction

## Overview(和訳)

<summary>
MITとハーバードのブロード研究所内のプロジェクトであるコネクティビティマップ、ハーバードのイノベーション科学研究所（LISH）、および統合ネットワークベースのセルラー署名のNIH共通基金ライブラリ（LINCS）は、この課題を次の目標で提示します。 MoA予測アルゴリズムの改善を通じて医薬品開発を推進します。
</summary>
<details>
The [Connectivity Map](https://clue.io/), a project within the Broad Institute of MIT and Harvard, the [Laboratory for Innovation Science at Harvard (LISH)](http://lish.harvard.edu/), and the [NIH Common Funds Library of Integrated Network-Based Cellular Signatures (LINCS)](http://lincsproject.org/]), present this challenge with the goal of advancing drug development through improvements to MoA prediction algorithms.
</details>

<summary>
薬が効く仕組みとはどのようなものなので消化?また、その仕組みはなぜ大事なのでしょうか?
</summary>
<details>
What is the Mechanism of Action (MoA) of a drug? And why is it important?
</details>

<summary>
従来、科学者たちは天然物や伝統的な治療法にひらめきを得て、薬を作ってきました。アメリカではアセトアミノフェンとして知られているパラセタモールなどのとても一般的な薬は数十年もの間、その薬理学的な働きに由来する生物学的なメカニズムが理解されていないまま臨床の場で使われてきました。今ではより強力な技術が発見されたため、薬を見つける行為は昔の偶然に頼るやり方から全く変わり、病気の生物学的なメカニズムに基づいたものになりました。
</summary>
<details>
In the past, scientists derived drugs from natural products or were inspired by traditional remedies. Very common drugs, such as paracetamol, known in the US as acetaminophen, were put into clinical use decades before the biological mechanisms driving their pharmacological activities were understood. Today, with the advent of more powerful technologies, drug discovery has changed from the serendipitous approaches of the past to a more targeted model based on an understanding of the underlying biological mechanism of a disease. In this new framework, scientists seek to identify a protein target associated with a disease and develop a molecule that can modulate that protein target. As a shorthand to describe the biological activity of a given molecule, scientists assign a label referred to as mechanism-of-action or MoA for short.
</details>
<summary>
どのようにして、新しい薬の効く仕組みは決まるのでしょうか?
</summary>
<details>    
How do we determine the MoAs of a new drug?
</details>
<summary>
一つのやり方は人間の細胞のサンプルに対して薬を投与してみて、遺伝子発現のライブラリや既知のMoAを持つ薬物の細胞生存パターンなど、膨大なゲノムデータベースの中の既知のパターンと類似性を見つけるアルゴリズムでその細胞の反応を分析するというものです。
</summary>
<details>
One approach is to treat a sample of human cells with the drug and then analyze the cellular responses with algorithms that search for similarity to known patterns in large genomic databases, such as libraries of gene expression or cell viability patterns of drugs with known MoAs.
</details>
<summary>
このコンペでは、遺伝子発現と細胞生存率を結びつけたユニークなデータにアクセスすることが出来ます。このデータは、100の異なる細胞の種類(したがって、特定の薬により適している細胞のタイプどれなのかを見極める必要がある問題を事前に解決しています)。それに加えこのデータセットでは、5000を超える薬のMoAの説明にアクセスすることが出来ます。
</summary>
<details>
In this competition, you will have access to a unique dataset that combines gene expression and cell viability data. The data is based on a new technology that measures simultaneously (within the same samples) human cells’ responses to drugs in a pool of 100 different cell types (thus solving the problem of identifying ex-ante, which cell types are better suited for a given drug). In addition, you will have access to MoA annotations for more than 5,000 drugs in this dataset.
</details>
<summary>
慣習的に、データセットはテストデータと訓練データに分けられています。そのため、**あなたに与えられたタスクは、訓練データを用いて一つ以上のテストデータの各ケースに対してを複数あるMoAクラスのラベルのどれに当たるかをラベル付けすることです**。薬は、複数のMoAラベルを持つ可能性があるため、タスクは正式にはマルチラベル分類問題であることに気をつけてください。
</summary>
<details>
As is customary, the dataset has been split into testing and training subsets. Hence, your task is to use the training dataset to develop an algorithm that automatically labels each case in the test set as one or more MoA classes. Note that since drugs can have multiple MoA annotations, the task is formally a multi-label classification problem.
</details>
<summary>
ソリューションの精度はどのように評価するのでしょうか?
</summary>
<details>
How to evaluate the accuracy of a solution?
</details>
<summary>
MoAラベルに基づき、ソリューションの精度は各薬のMoAラベルのペアに適用された対数誤差関数の平均値によって評価されます。
</summary>
<details>
Based on the MoA annotations, the accuracy of solutions will be evaluated on the average value of the [logarithmic loss function](https://www.kaggle.com/c/lish-moa/overview/evaluation) applied to each drug-MoA annotation pair.
</details>
<summary>
もし成功すれば、あなたはどの細胞の特徴を考慮した化合物のMoAの予測アルゴリズムの開発に貢献したことになります。このことは科学者たちの創薬のプロセスに役立ちます。
</summary>
<details>
If successful, you’ll help to develop an algorithm to predict a compound’s MoA given its cellular signature, thus helping scientists advance the drug discovery process.
</details>
<summary>
このコンペはコードコンペです。詳細はコード要件を参照してください。
</summary>
<details>
This is a Code Competition. Refer to [Code Requirements](https://www.kaggle.com/c/lish-moa/overview/code-requirements) for details.
</details>
