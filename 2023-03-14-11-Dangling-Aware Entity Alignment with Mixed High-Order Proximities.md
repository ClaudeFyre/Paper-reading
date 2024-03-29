## Paper:5




1. Title: Dangling-Aware Entity Alignment with Mixed High-Order Proximities (混合高阶相似度感知知识图谱实体对齐)

2. Authors: Jia Zhu, Rong Pan, Chengjiang Li, Yujian Guo, Jie Zhang, Jun Gao

3. Affiliation: 华东师范大学 (East China Normal University)

4. Keywords: Knowledge graphs, Entity alignment, Dangling entity problem, High-order proximities.

5. Url: http://arxiv.org/abs/2205.02406v1 , Github: None

6. Summary: 
- (1):本文研究了知识图谱实体对齐中的悬挂实体问题，对此提出了一种混合高阶相似度感知框架。悬挂实体是指在一个知识图谱中，找不到对应实体的实体。相比于之前忽略悬挂实体的实体对齐方法，本文提出的方法更为实际。 
- (2):以往的实体对齐方法忽略了悬挂实体的存在，无法实际支持物理世界中的知识图谱对齐任务。本文提出的方法引入了两种高阶相似度作为衡量依据，即用于最近邻子图中的局部高阶相似度和嵌入空间中的全局高阶相似度。 
- (3):文章提出了一种混合高阶相似度感知框架，用于悬挂实体检测和实体对齐。该框架将最近邻子图中的局部高阶相似度和嵌入空间中的全局高阶相似度混合在一起，以提高实体对齐的准确性。 
- (4):在两个评估设置下进行的大量实验证明了该方法的有效性，表现出更准确的悬挂实体检测和更好地匹配可匹配实体。同时，该方法也缓解了悬挂实体对齐中的hubness问题。
7. Methods: 

- (1): 本文提出了一种混合高阶相似度感知框架，用于悬挂实体检测和实体对齐。该方法引入了两种高阶相似度作为衡量依据，即用于最近邻子图中的局部高阶相似度和嵌入空间中的全局高阶相似度。

- (2): 为了利用嵌入空间中的全局高阶相似度，本文提出了一种基于Optimal Transport的方法，用于全局匹配可匹配源实体与目标实体之间的嵌入向量的分布。此外，为了便于检测悬挂实体，该方法还鼓励源和目标KG中悬挂实体向量的分布之间有更大的距离。该方法将Wasserstein距离用于量化源和目标图谱之间的差异。为了解决Wasserstein距离的最优传输问题，文章采用了Wasserstein GAN作为实现工具。此外，为了区分悬挂实体，该方法将悬挂实体看作两个嵌入分布中不同的部分。

- (3): 本文还提出一种基于局部高阶相似度的悬挂实体检测方法。相比于以往的方法，该方法考虑了最近邻子图中的二阶相似度，并通过设计一个feed-forward神经网络来区分悬挂实体和可匹配实体。为了使损失函数对悬挂实体起作用，文章提出了一种用于悬挂实体的训练集和损失函数，该函数将转换后的悬挂实体向量的分布与目标实体向量的分布之间的差异最大化。此外，本文还提出了邻域组件分析（NCA）损失函数来缓解hubness问题。在实验分析中，本文还采用了一种结合局部高阶相似度和嵌入空间中的全局高阶相似度的方法，最终验证了该方法的有效性。





8. Conclusion:

- (1): 本文的意义在于，针对知识图谱实体对齐中的悬挂实体问题，提出了一种混合高阶相似度感知框架。该框架引入了两种高阶相似度，即局部高阶相似度和全局高阶相似度，在悬挂实体检测和实体对齐任务中具有较高的实用性，对于实现物理世界中的知识图谱对齐任务有着很大的应用前景。
                     
- (2): 创新点方面，本文提出了一种混合高阶相似度感知框架，是针对悬挂实体问题进行了深入研究，有一定的创新性。性能方面，经过大量实验证明，该方法比以往忽略悬挂实体的实体对齐方法在悬挂实体检测和实体匹配方面更为准确，具有较高的性能水平。工作量方面，本文提出了多种检测和匹配方法，需要一定的工作量在实现和验证方面。




