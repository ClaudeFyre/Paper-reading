## Paper:43




1. Title: Cross-lingual Knowledge Graph Alignment via Graph Matching Neural Network (通过图匹配神经网络实现跨语言知识图谱对齐)

2. Authors: Xiucheng Li, Shuangyin Li, Jingyuan Zhang, Junchi Yan, Philip S. Yu

3. Affiliation: 中国科学院大学 (University of Chinese Academy of Sciences)

4. Keywords: Cross-lingual knowledge graph alignment, Graph matching, Neural network, Attention mechanism

5. Url: http://arxiv.org/abs/1905.11605v3, Github: https://github.com/syxu828/Crosslingula-KG-Matching

6. Summary:
- (1): 本文旨在解决跨语言知识图谱中实体匹配问题。
- (2): 过去的跨语言知识图谱对齐方法仅依赖于单语言知识图谱结构信息推导实体嵌入, 难以匹配在两个知识图中包含不同事实的实体。本文提出通过对主题实体子图进行图匹配来表示带有KG上下文的实体, 并采用基于图注意力的方法来解决图的匹配问题。相较于以往的方法, 它可以更好地匹配在两个KG中具有不同事实的实体。 
- (3): 本文提出了主题实体子图来表示实体及其上下文信息，提出了基于图注意力的策略来进行跨语言知识图的实体匹配，利用图上GCN算法来将所有实体的匹配信息传递至整个图，通过利用二者之间的节点匹配信息从而得出全局相似度，同时不依赖于单语言知识图谱结构的信息。
- (4): 本文的方法在跨语言相对论知识图谱数据集上实现了较好的表现，结果表明该方法能够更好地捕捉实体上下文信息，并超过了以往的对比方法。
7. Methods:

- (1): 本文旨在解决跨语言知识图谱中实体匹配问题。在这个问题上，过去的跨语言知识图谱对齐方法仅依赖于单语言知识图谱结构信息推导实体嵌入, 难以匹配在两个知识图中包含不同事实的实体。
- (2): 本文提出通过对主题实体子图进行图匹配来表示带有KG上下文的实体, 并采用基于图注意力的方法来解决图的匹配问题。相较于以往的方法, 它可以更好地匹配在两个KG中具有不同事实的实体。本文提出了主题实体子图来表示实体及其上下文信息，提出了基于图注意力的策略来进行跨语言知识图的实体匹配，利用图上GCN算法来将所有实体的匹配信息传递至整个图，通过利用二者之间的节点匹配信息从而得出全局相似度，同时不依赖于单语言知识图谱结构的信息。
- (3): 本文介绍的方法包含两个关键步骤，图编码和图匹配。首先，对于每个语言的知识图谱，本文对其进行预处理，通过识别出主题实体及其相邻节点构建主题实体子图。其次，使用基于图注意力的模块来进行图的匹配。该模块将两个主题实体子图作为输入，并生成一个图表示两个图的相似度，并使用HopGCN2结构来优化全部实体的预测，以便获取最终的跨语言知识图谱对齐结果。
- ......





8. Conclusion:

- (1): 本文提出的跨语言知识图谱对齐方法具有很高的应用价值，可以在多语言信息共享，知识推理等领域中得到广泛应用。该方法相较于传统的方法，更好地捕捉实体上下文的信息，并成功解决了跨语言知识图谱中的实体匹配问题。

- (2): 创新点：本文提出了通过对主题实体子图进行图匹配的方法来表示带有KG上下文的实体，并采用基于图注意力的策略进行跨语言知识图谱的实体匹配。相较于以往的方法，这种方法可以更好地匹配在两个知识图中具有不同事实的实体。性能：在跨语言相对论知识图谱数据集上实现了较好的表现，结果表明该方法能够更好地捕捉实体上下文信息，并超过了以往的对比方法。工作量：在实验中，该方法对图的匹配需要较高的计算复杂度，但可以在较短时间内得到良好的实验结果。




