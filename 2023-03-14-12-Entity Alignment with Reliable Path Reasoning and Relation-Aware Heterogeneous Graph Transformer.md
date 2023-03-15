## Paper:67




1. Title: Entity Alignment with Reliable Path Reasoning and Relation-Aware Heterogeneous Graph Transformer (使用可信路径推理和关系感知异构图变换的实体对齐)

2. Authors: Zhangyuan Tian, Jialian Li, Quan Wang, Jianzhu Ma, Jia Wu

3. Affiliation: Zhangyuan Tian, Tsinghua University

4. Keywords: Entity Alignment, Knowledge Graphs, Relation Path, Heterogeneous Graph Transformer.

5. Urls: http://arxiv.org/abs/2205.08806v2, Github: None

6. Summary:

- (1): 在知识图谱领域，不同知识图谱间的联系往往断断续续，难以整合，实体对齐（EA）就是一项将不同知识图谱中的同义实体联系起来的重要任务。

- (2): 过去的方法往往未考虑知识图谱的异构性，即网络节点之间的异构特征；另外，也忽略了实体的路径结构信息，这些限制了 EA 方法的表现。本文提出了一种更有效的 EA 框架，RPR-RHGT，整合了关系和路径结构信息，以及知识图谱中的异构信息。本文首次提出了一种初始可信路径推理算法，它可以从知识图谱的关系结构中生成有利于 EA 任务的路径结构，从而充分利用了知识图谱中的丰富信息。同时，为了有效捕捉实体邻域的异构特征，本文设计了一个关系感知异构图变换器，用于模拟知识图谱的关系和路径结构。在三个知名数据集上的 extensive 实验表明，RPR-RHGT 显著优于 11 种现有方法，在 Hits@1 上的表现高出最佳基线达 8.62%。

- (3): 本文的贡献主要包括两方面：一是提出了 RPR-RHGT 框架，它将关系和路径结构信息与 KG 中的异构信息融合在一起，能够有效提高 EA 的精度和鲁棒性；二是提出了可信路径推理算法 RPR，它可以根据关系结构提取出有助于 EA 任务的路径结构信息。

- (4): 本文的方法在三个知名数据集上的 extensive 实验表明，RPR-RHGT 方法在 EA 任务上表现均优于其它方法，能够可靠地实现实体相互对齐。





8. Conclusion:

- (1): 本文提出的实体对齐框架 RPR-RHGT 同时考虑了实体的关系和路径结构信息，以及知识图谱的异构性，实现了可靠的实体对齐。文章所提出的初始可信路径推理算法 RPR 则有望成为后续相关工作的研究热点。

- (2): 创新点：文章提出了一种综合考虑实体关系、路径结构和异构性的实体对齐框架，同时首次提出了可信路径推理算法，这将为实体对齐领域研究提供新的思路。性能：RPR-RHGT 在三个知名数据集上的 extensive 实验表明，实现了较高的精度表现。工作量：虽然文章所提出的算法 RPR-RHGT 的计算复杂度较高，但是其所取得的实验结果表明，仍然具备实用价值。




