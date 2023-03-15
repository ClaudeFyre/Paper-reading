## Paper:63




1. Title: Collective Entity Alignment via Adaptive Features（通过自适应特征的集体实体对齐）

2. Authors: Wen Zhang, Xiang Zhao*, Hongbin Ye, Wei Fan, Yiqun Liu, Xiaojiang Liu, Peiran Ren, Jiandong Wang

3. Affiliation: Xiang Zhao is from National University of Defense Technology (国防科技大学)

4. Keywords: entity alignment, knowledge graphs, stable matching problem, deferred acceptance algorithm

5. Urls: http://arxiv.org/abs/1912.08404v3

6. Summary:

- (1): 本文研究领域为实体对齐(reinforcement learning)，旨在发现描述同一真实对象但存在于不同知识图谱(KGs)中的实体，并已应用于KG构建和集成。

- (2): 当前的解决方案仅考虑实体之间的独立性，忽视了实体之间的相互依赖性。本文针对此提出了一种集体实体对齐框架，利用自适应特征来捕捉异构KG中实体之间相似性的不同方面，进而将EA (Entity Alignment)定义为稳定匹配问题 (SMP)，采用deferred acceptance算法来进行决策。相较于基于嵌入的EA方法，本文方法可以更好地建模实体之间的依赖关系。

- (3): 本文的研究方法是建立集体实体对齐(Collective Entity Alignment, CEA)框架，在自适应特征的基础上，将稳定匹配问题与deferred acceptance算法相结合。

- (4): 本文在跨语言和单语言EA基准测试中，与11种基线方法进行了比较，验证了CEA方法的有效性和优越性。





8. Conclusion: 

- (1): 本文提出了一种新的集体实体对齐方法，旨在提高异构知识图谱的融合效率，具有一定的研究价值。

- (2): 创新点：提出了自适应特征和集体实体对齐框架，可更好地捕捉实体间的依赖关系，提高了对齐效率；性能：实验结果表明，在跨语言和单语言EA基准测试中，本文方法优于11种基线方法；工作量：未给出详细的工作量数据，需要在后续研究中探究。




