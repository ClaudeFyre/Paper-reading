## Paper:21






1. Title: EventEA: Benchmarking Entity Alignment for Event-centric Knowledge Graphs (EventEA: 以事件为中心知识图谱实体对齐基准)

2. Authors: Xiaoke Tian, Xi Chen, Yuanzhuo Wang, Hong Qin, Zhiyuan Liu, Jia Song

3. Affiliation: Xiaoke Tian - Department of Computer Science and Technology, Tsinghua University, Beijing, China (夏可可 - 清华大学计算机科学与技术系，中国北京), others - unknown

4. Keywords: Entity Alignment, Knowledge Graphs, Event-centric, Embedding-based, Benchmarking

5. Urls: Paper - http://arxiv.org/abs/2211.02817v1, Github - None

6. Summary: 

- (1): 本文的研究背景为，进行不同知识图谱中实体对齐，并比较基于嵌入的方法在这一领域中的表现。

- (2): 过去的实体对齐方法主要集中在属性的相似性或基于关系语义的逻辑推理上，最近的研究则更多地关注编码方法，这是由于编码方法可以解决跨不同知识图谱的符号异构问题。但是，本文发现了现有数据集中存在两个问题：即关系三元组中等同图结构；属性三元组中异构性不足。本文从事件中心的知识图谱出发，构建了一个具有异构关系和属性的对齐数据集，来评估现有流行的方法，并发现它们并不能取得良好的性能。同时本文也提出了一种用于实体对齐的基于时间的文本编码方法。

- (3): 本文提供了一个具有异构关系和属性的新颖的事件中心数据集 EventEA，该数据集可用于评估与实体对齐相关的任何工作。文章还提出了一种基于时间的文本编码方法，来解决属性异构性的问题。

- (4): 在 EventEA 上的实验证明，现有的实体对齐方法在面对异构关系和属性时表现非常糟糕，而文章提出的方法在保证效率的情况下表现相当不错。这表明 EventEA 是一种更有效的数据集，可以帮助开发更有效的实体对齐方法。
7. Methods:

- (1): 本文提出了一种基于事件中心的知识图谱的对齐数据集 EventEA，该数据集包含了异构关系和属性的实体对齐问题。同时本文提出了一种基于时间编码的方法，以解决属性异构性的问题。

- (2): 对于基于事件中心的对齐数据集 EventEA，本文提出了一种基于时间注意力机制的实体对齐模型。该模型首先将时间嵌入进行文本编码，然后使用注意力机制对编码后的文本进行加权求和，生成时间感知的向量表示；接着，使用同样的机制对属性嵌入进行文本编码，并得到属性感知的向量表示。最后将时间和属性的向量表示进行线性组合，并使用异质性映射方法进行实体对齐。

- (3): 作者还提出了一种基于规则的时间识别器，通过查找常见的时间格式识别时间信息。在实验中，针对 EventEA 数据集，实验证明了作者提出的实体对齐方法在性能上的优越性。





8. Conclusion:

- (1): 本文旨在解决知识图谱实体对齐中存在的问题，提出了一种新颖的基于事件中心的对齐数据集 EventEA 和一种基于时间编码的实体对齐方法，可以有效地解决属性异构性的问题。本文论证了 EventEA 泛化能力的优越性，也提出了一种具有实际应用价值的基于规则的时间识别器。

- (2): 创新点：EventEA 数据集是一个具有异构关系和属性的对齐数据集，针对性强，测试现有实体对齐方法的性能，为实体对齐研究提供了新的思路。基于时间编码的实体对齐方法和基于规则的时间识别器也为实体对齐方法的改进提供了新的方向。性能：本文提出的方法在 EventEA 上的实验表明，基于时间编码的实体对齐方法比现有流行的方法效果更好，并且具有计算性能的优点。同时，本文提供的时间识别器也能有效地提高时间处理的效率。工作量：本文中提出的方法和数据集构建都是具有一定工作量的，但是相对于现有的实体对齐工作，是可承受的，具有一定的推广价值。




