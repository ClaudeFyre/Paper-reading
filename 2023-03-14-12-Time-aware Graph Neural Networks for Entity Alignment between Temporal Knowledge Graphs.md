## Paper:27






1. Title: Time-aware Graph Neural Networks for Entity Alignment between Temporal Knowledge Graphs (基于时间感知图神经网络的时态知识图谱实体对其方法)

2. Authors: Dongjun Wei, Jie Zhang, Yajuan Lyu, Huiming Wang, Shengqi Yang, Xia Du

3. Affiliation: 东南大学计算机科学与工程学系 (Department of Computer Science and Engineering, Southeast University)

4. Keywords: Entity alignment, Graph Neural Networks, Temporal Knowledge Graphs, Time-aware attention mechanism, Multi-relation information

5. Urls: Paper: http://arxiv.org/abs/2203.02150v2; Github: None

6. Summary: 

- (1):该论文探讨知识图谱（KGs）中实体对齐问题，特别是针对时间知识图谱（TKGs）提出解决方案。

- (2):以往的实体对齐方法，如基于嵌入的方法，忽略了实体之间时间信息的作用，造成实体对齐效果不佳。本论文通过提出一种基于图神经网络的TEA-GNN（Time-aware Entity Alignment approach based on Graph Neural Networks）方法，将实体、关系和时间戳嵌入到一个向量空间中，结合图神经网络学习实体表示，进一步用具有时间感知的注意机制，将关系和时间信息实现结合。实验结果证明，该方法显著优于现有方法。

- (3):本论文提出了一个基于图神经网络的时态知识图谱实体对其方法，实现对实体对齐问题的解决。

- (4):本文的方法在多个真实世界的TKGs数据集中进行了实验，结果显示性能显著优于现有方法，且通过不同的实验设置得出不同的结论，拓展了该领域的相关研究。
7. Methods:

- (1): 本文提出了一种基于图神经网络的时态知识图谱实体对齐方法，该方法将实体、关系和时间戳嵌入到一个向量空间中，同时结合图神经网络学习实体表示，采用具有时间感知的注意机制，将关系和时间信息实现结合。

- (2): 为了整合关系方向信息，本文将每个关系r生成反关系r-1，进一步扩展关系集合R，在时间戳和关系中采用正交变换的时间感知注意机制，根据它们之间的关系和时间信息为不同的相邻节点赋予权重。

- (3): 本文还提出了一种基于多视图表示的实体对齐方法，通过将不同视图的表示运用到距离函数中，预测实体对齐。实验表明，该方法相较于现有方法有显著提升，成功解决了实体对齐问题。





8. Conclusion: 
- (1): 本篇论文的意义在于提出了一种基于图神经网络的时态知识图谱实体对其方法，通过将实体、关系和时间戳嵌入到向量空间中，结合图神经网络学习实体表示，采用具有时间感知的注意机制，将关系和时间信息实现结合。该方法成功地解决了实体对齐问题，为时态知识图谱实体对齐提供了新的解决方案。

- (2): 创新点：本文提出了一种将时间信息嵌入实体对齐过程中的图神经网络模型，提高了实体对齐的准确性；性能：该方法在多个真实世界的TKGs数据集中经过了实验，结果表明该方法性能显著优于现有方法；工作量：本文针对实体对齐问题提出了两种不同的方法，但是对于实验的数据预处理部分，属于较为繁琐的部分。




