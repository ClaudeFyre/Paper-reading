## Paper:45






1. Title: Ontology Alignment in the Biomedical Domain Using Entity Definitions and Context

2. Authors: Sahil Swami, Wei-Hung Weng, Kyle Lo, Huan Sun, Sameer Singh

3. Affiliation: Sahil Swami: Allen Institute for Artificial Intelligence

4. Keywords: Ontology alignment, Biomedical domain, Entity definitions, Context, Neural architecture, Supervised learning, UMLS Metathesaurus

5. Urls: Paper: http://arxiv.org/abs/1806.07976v1, Github: https://www.github.com/allenai/ontoemma/

6. Summary:

- (1): 本文的研究背景是在生物医学领域中的本体对齐问题。由于不同生物医学本体中对同一实体的描述不同，导致融合本体时需要对实体进行去重，本文提出了一种利用外部定义和上下文信息来丰富本体实体的方法，并将此方法用于本体对齐任务。

- (2): 过去的本体对齐方法主要依赖于实体的名称、同义词和实体之间的关系等特征。然而，在自然语言文本方面的利用仍然不够充分，文章提出了利用实体的定义和上下文信息以及神经网络的结构来改进本体对齐的任务。采用了UMLS多源本体兼容的框架，利用神经网络进行本体对齐。

- (3): 本文的研究方法主要是提出了一种能够使用实体定义和上下文信息的神经网络体系结构，用于本体对齐任务。其中，使用UMLS Metathesaurus来提取带有标签的数据进行监督式对本体对齐模型进行训练，并结合了维基百科和科技文章等外部资源来获取实体定义和上下文信息，最终采用二分类的神经网络模型来预测两个实体是否语义上等价。

- (4): 该方法在PubMed中进行测试，实验结果表明，使用本文提出的方法，相应指标的F1-score为0.69，可以取得与SOTA系统中基于实体的匹配器相当的成绩，并且该方法易于实现并具有良好的泛化性能。
7. Methods: 

- (1): 本文采用了UMLS多源本体兼容的框架，并结合了维基百科和科技文章等外部资源来获取实体定义和上下文信息。

- (2): 为了处理不同本体的实体描述不同的问题，文章提出了一种利用外部定义和上下文信息来丰富本体实体的方法，并通过二分类的神经网络模型来预测两个实体是否语义上等价。

- (3): 实验中，本文使用了监督式学习来训练本体对齐模型，使用UMLS Metathesaurus来提取带有标签的数据来进行训练，并采用了二分类的神经网络模型来预测两个实体是否语义上等价。

- (4): 本文使用了PubMed中的数据集来评估本体对齐的性能，并且表明本文方法的F1得分为0.69，可以取得与SOTA系统中基于实体的匹配器相当的成绩。





8. Conclusion:

- (1): 本文提出了一种利用实体定义和上下文信息的方法来丰富本体实体，进而改进本体对齐的性能。对于生物医学领域这样实体描述不同的领域，本文方法可以提高本体对齐的准确率。

- (2): 创新点：本文采用了实体定义和上下文信息来改进本体对齐任务，从而提高任务效率。性能：本文提出的方法在PubMed中得到了与SOTA系统中基于实体的匹配器相当的成绩。工作量：本文方案易于实现，而且具有良好的泛化性能。




