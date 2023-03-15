## Paper:46




1. Title: Relation-Aware Entity Alignment for Heterogeneous Knowledge Graphs（面向异构知识图谱的关系感知实体对齐）

2. Authors: Xiaobin Hong, Chengjiang Li, Maximilien Servajean, Si Wu, Jie Tang

3. Affiliation: Xiaobin Hong (Tsinghua University)

4. Keywords: Entity Alignment, Knowledge Graph, Relation Awareness, Graph Convolutional Network

5. Urls: Paper: http://arxiv.org/abs/1908.08210v1, Github: None

6. Summary:

- (1): 本文针对知识图谱中真实世界实体在不同知识图谱中的链接问题进行研究。

- (2): 先前的面向知识图谱实体对齐的嵌入式方法通常不能很好地捕捉多关系知识图谱中的复杂关系信息。因此，本论文提出了一种新的方法，即关系感知双图卷积网络（RDGCN），通过注意关系来整合关系信息，通过构建邻域结构来学习更好的实体表示。 

- (3): 本文提出的RDGCN通过将知识图和其对偶图之间的关系进行注意交互来建模实体之间的语义关系。 进一步使用图形卷积操作来学习实体嵌入特征。

- (4): 在三种跨语言数据集上进行的实验结果表明，本文方法在学习更好的知识图谱表示方面比现有方法提供更好和更健壮的结果，验证了方法的有效性。







8. Conclusion: 

- (1): 本文针对异构知识图谱中不同图之间实体对齐问题提出了一种新的方法，即关系感知双图卷积网络（RDGCN）。该方法可以有效地整合关系信息，通过构建邻域结构来学习更好的实体表示。在三个跨语言数据集上进行的实验结果表明，该方法比现有方法提供更好和更健壮的结果，验证了方法的有效性。

- (2): 创新点：该文提出了一种新的方法RDGCN来解决实体对齐问题，在注意关系的基础上，进一步使用图形卷积操作来学习实体的嵌入特征。性能：通过在跨语言数据集上的实验结果表明，该方法在实体对齐方面比现有方法提供更好和更健壮的结果。工作量：该方法的具体工作流程相对简单易懂，但需要较多的实验验证来完成。




