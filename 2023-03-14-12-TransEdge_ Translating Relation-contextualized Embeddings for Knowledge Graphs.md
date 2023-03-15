## Paper:74




1. Title: TransEdge: Translating Relation-contextualized Embeddings for Knowledge Graphs (基于边嵌入的知识图谱关系表示模型)

2. Authors: Zhenyu Sun, Wei Hu, Chengming Zhang, Jie Yang, Rongrong Ji, and Xiaopeng Zhang

3. Affiliation: 中国科学院深圳先进技术研究院 (Chinese Academy of Sciences, Shenzhen Advanced Technology Research Institute)

4. Keywords: Knowledge Graphs, Embeddings, TransEdge, Entity Alignment, Link Prediction

5. Urls: Paper: http://arxiv.org/abs/2004.13579v1, Github: None

6. Summary: 

- (1): 本文研究的背景为如何学习到高质量的知识图谱（KG）关系表示。如何将实体和关系先转化为向量表示，再通过向量的相似性来计算关系，是目前学术上研究的热点之一。

- (2): 过去的方法大多采用将关系视为线性或者二次映射，缺乏对KG中多样关系结构的充分表达，难以准确捕捉在不同上下文中的关系含义，约束精度，本文提出了基于边嵌入的TransEdge关系表示模型，将关系表示上下文化，按照头尾实体对的不同，对每个关系作出差异化表达，以便更好地反映KG中的结构特征，并借鉴TransE的思想，构建了边嵌入，建立了实体嵌入之间的边界限制关系。TransEdge在不同的预测任务中表现出了其优点。

- (3): 本文提出了边嵌入的概念，并借鉴TransE的思想，在头尾实体对不同的情况下建立嵌入和实体之间的边界限制关系。

- (4): 本文在 KG 实体对比对和链接预测两个任务上进行了实验，结果显示 TransEdge 在对齐实体上表现较好，同时在链接预测中也取得了很好的效果，证明了它的有效性。
7. Methods: 

- (1): 本文提出了一种基于边嵌入的知识图谱（KG）关系表示模型TransEdge，它将关系表示上下文化，按照头尾实体对的不同，对每个关系作出差异化表达，以便更好地反映KG中的结构特征。该模型借鉴了TransE的思想，构建了边嵌入，建立了实体嵌入之间的边界限制关系。

- (2): 为了验证TransEdge的有效性，本文进行了两项实验任务：KG实体对齐和链接预测。对于实体对齐，TransEdge表现较好，并在链接预测中取得了很好的效果。

- (3): 本文还将TransEdge与传统实体对齐方法LogMap进行比较，发现LogMap表现优异，但将两者结果进行组合后效果更佳。

- (4): TransEdge的核心思想是将关系表示上下文化，用边嵌入表达关系的多样性，并且有效解决了KG中多种关系结构的问题。





8. Conclusion: 

- (1): 本文的意义在于提出基于边嵌入的TransEdge关系表示模型，用于学习知识图谱中的关系表示。该模型能够更好地反映KG中的结构特征，同时与传统方法相比，具有更好的实验效果。

- (2): 创新点：本文创新地提出了边嵌入的概念，用于表示关系的多样性，以及在头尾实体对不同的情况下建立嵌入和实体之间的边界限制关系。性能方面，实验结果表明，TransEdge 在对齐实体和链接预测中都表现较好，证明了其有效性。工作量方面，本文对两项实验任务展开了详细的实验分析，说明了TransEdge的优点和局限性。

- (3): 综上所述，本文提出的TransEdge模型在知识图谱关系表示领域具有较大的创新性和实用性，具有一定的优势和局限性，可以为相关领域的研究者提供新的研究思路和方法，并为语义技术的应用提供有力的支持。




