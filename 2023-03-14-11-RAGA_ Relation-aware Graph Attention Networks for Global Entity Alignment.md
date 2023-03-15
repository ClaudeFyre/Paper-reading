## Paper:16




1. Title: RAGA: Relation-aware Graph Attention Networks for Global Entity Alignment（关系感知图注意力网络用于全局实体对齐）


2. Authors: Rong Zhu, Xiaozhong Liu, Ce Zhang, Qiongkai Xu, Rui Zhang


3. Affiliation: 中国科学院计算技术研究所 (Institute of Computing Technology, Chinese Academy of Sciences)


4. Keywords: Entity alignment, multi-source knowledge graphs, graph neural networks, attention mechanism


5. Urls: Paper: http://arxiv.org/abs/2103.00791v1 ; Github: None


6. Summary:

- (1): 该论文的研究背景是在现有的知识图谱（KG）集成任务中，需要对不同知识图谱的实体进行全局对齐以实现更完整的知识表示。

- (2): 过去的方法主要采用基于嵌入的实体对齐方法，这些方法通过将实体和关系编码为向量空间来计算相似度，但这些方法不足的地方在于不充分考虑实体之间的多重关系和 KG 结构信息，而且目前的实体对齐方法常常采用本地对齐策略，存在无法合理匹配多对一实体的问题。本文提出一种新的框架，即 RAGA，采用关系感知图注意力网络（Relation-aware Graph Attention Networks）来捕捉实体和关系之间的交互，较好地解决了上述问题。

- (3): 该文提出的 RAGA 框架具有两个核心组件：自注意力机制和全局对齐算法。其中自注意力机制能够将实体信息传递到关系上，并且再将关系信息聚合回实体；全局对齐算法则使用细粒度相似矩阵精细地计算实体之间的一一对齐关系。

- (4): 文章的实验结果表明，RAGA 在三个跨语言实体对齐数据集上取得了比其他方法更好的性能，证明了该方法的有效性。
7. Methods:

- (1): 该论文提出了一种新的实体对齐框架 RAGA，整体思路是采用关系感知图注意力网络来捕捉实体和关系之间的交互，同时使用全局对齐算法来计算实体之间的一一对齐关系。

- (2): 该方法的具体实现分为两个核心组件，即自注意力机制和全局对齐算法。自注意力机制可将实体信息传递到关系上，并将关系信息聚合回实体，全局对齐算法则使用细粒度相似矩阵精细地计算实体之间的一一对齐关系。

- (3): 在数据预处理方面，将不同知识图谱转化为相同格式的实体-关系-实体三元组（triple），同时使用在知识图谱中出现的实体描述信息、关系描述信息和属性值信息进行特征表示。在训练时，使用三个不同的损失函数（包括 KG 嵌入训练、局部对齐监督和全局对齐监督）来逐步训练模型。

- (4): 在实验方面，文中使用三个公开跨语言实体对齐任务数据集进行了评测，并与现有的多种实体对齐方法进行了比较。实验结果表明，提出的 RAGA 方法比其他方法在性能上更加优秀。





8. Conclusion: 

- (1): 本论文提出了一种新的实体对齐框架 RAGA，旨在解决现有知识图谱集成任务中全局对齐问题和多重关系问题，具有重要的研究意义。
  
- (2): 创新点方面，该框架采用了关系感知图注意力网络和全局对齐算法，可以充分利用多重关系和全局信息进行实体对齐。在性能方面，在三个跨语言实体对齐数据集上，该方法表现出比其他方法更好的性能。在工作量方面，虽然该方法需要逐步训练模型，但是具体实现步骤介绍的详细，易于操作。





