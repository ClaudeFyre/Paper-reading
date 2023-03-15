## Paper:23




1. Title: MEAformer: Multi-modal Entity Alignment Transformer for Meta Modality Hybrid (中文翻译：面向元模态混合的多模实体对齐变换器)

2. Authors: Wenhan Chen, Yifan Qiao, Yu Zhu, Wei Zhang, Hao Peng

3. Affiliation: Wenhan Chen - 阿里巴巴人工智能实验室

4. Keywords: multi-modal entity alignment, meta-learning, transformer, modality fusion, cross-modal

5. Urls: http://arxiv.org/abs/2212.14454v2, Github: None

6. Summary:

- (1): 本文研究的背景是多模态实体对齐，希望能够根据实体相关联的图像，发现不同知识图谱中的相同实体。

- (2): 过去的方法主要集中在设计适当的跨知识图谱模态融合范式，但是忽略了个体模式偏好的变化，影响模型的鲁棒性。本文提出了MEAformer方法，通过动态预测模态之间的权重，进一步增加多模态实体对齐模型的鲁棒性。此外，还提出了具有模式感知的硬实体重放策略，进一步加强了模型对模糊实体细节的鲁棒性。

- (3): 本文提出了一种名为MEAformer的新颖方法，采用元学习算法，在实体层面上生成合理的多模态实体混合特征，并在动态交叉Attention网络中预测模态之间的相互关联系数，实现模态自适应。

- (4): 采用的模型在自监督、无监督、迭代和低资源等多种训练场景下取得了最先进的性能。此外，该模型的参数数量较少，计算速度优秀，可解释性较好。
7. Methods:

- (1): 本文的研究方法是针对多模态实体对齐这一问题，提出了一种新颖的MEAformer模型。该模型采用元学习算法，在实体层面上生成合理的多模态实体混合特征，并在动态交叉Attention网络中预测模态之间的相互关联系数，实现模态自适应。

- (2): 该模型包括两个主要部分：多模态知识嵌入和元模态混合。首先，通过Graph Neighborhood Structure Embedding、Relation, Attribute, Visual 和 Surface Embedding等方法，将每个模态的实体嵌入到低维向量空间中。之后，利用meta modality hybrid(MMH)模块动态生成实体级元权重，将多模态嵌入的结果进行加权平均，得到实体级别的多模态表示。该模型还采用modal-adaptive contrastive learning (MACL)方法对少量标记样本进行训练，获得更好的任务效果。

- (3): 与其他相关工作相比，MEAformer能够根据实际情况自适应地调整每个模态的权重，并针对元素的异构关系进行建模，从而实现更好的多模态实体对齐性能。

- (4): 该模型在多个实验中表现出较好的性能，并具有参数数量较少、计算速度优秀、可解释性较好的优点。





8. Conclusion:

- (1): 本文提出了一种元模态混合的多模态实体对齐变换器——MEAformer。针对多模态知识图谱实体对齐问题，该方法可以自适应地调整每个模态的权重，建模元素异构关系，具有较好的性能表现。

- (2): 创新点：本文提出了一种元模态混合的方法，采用动态交叉Attention网络对多模态实体对齐进行建模。在任务性能方面，MEAformer在多个实验下表现出较好的性能，并解决了传统方法对模态偏好变化的问题。在工作量方面，该方法采用元学习算法，参数数量较少，计算速度优秀，并具有较好的可解释性。




