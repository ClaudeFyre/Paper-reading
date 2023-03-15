## Paper:4




1. Title: Conflict-Aware Pseudo Labeling via Optimal Transport for Entity Alignment

2. Authors: Chaoyu Guan, Xinxing Xu, Haishuai Wang, Jie Shao, Xiaohua Jia, Xiaodan Zhu

3. Affiliation: Chaoyu Guan, Xinxing Xu, Haishuai Wang, and Jie Shao are affiliated with the School of Cyber Engineering, Xidian University, China. Xiaohua Jia is affiliated with the School of Computer Science, Northwestern Polytechnical University, China, and Xiaodan Zhu is affiliated with the Department of Computer Science and Engineering, Shanghai Jiao Tong University, China.

4. Keywords: Entity Alignment, Optimal Transport, Conflict-Aware Pseudo Labeling, KG Embedding

5. Urls: http://arxiv.org/abs/2209.01847v2 or Github: None

6. Summary:

- (1): 该论文主要研究知识图谱实体对齐中的冲突问题，提出了一种基于最优输运的冲突感知伪标记模型来提高实体对齐效果。

- (2): 该论文中提到现有的知识图谱实体对齐方法都是将知识图谱映射到一个潜在的嵌入空间中，以捕捉实体间的内在语义，但当前的方法往往忽视了训练过程中的对齐冲突问题，从而限制了实体对齐的性能。论文作者对此问题提出了一种新的解决方案，即利用最优输运模型对对齐实体进行伪标记，并采用冲突感知的方法提高对齐精度。

- (3): 该论文提出了一种基于最优输运的冲突感知伪标记方法，该方法通过最小化总体输运成本保证一对一实体对齐，缓解了对齐冲突问题。论文中还设计了全局局部聚合的图卷积方法用于学习表达性的实体嵌入。

- (4): 论文作者的方法在多个基准数据集上进行了实验，并在有无先验对齐种子的情况下，均取得了优于现有最先进方法的结果。结果表明，该方法可以有效地提高实体对齐的精度，达到预期目标。
7. Methods: 

- (1): 本文提出的CPL-OT模型采用最优输运的伪标记方法来增强实体对齐的先验标记，以提高实体对齐效果。该方法包含两个部分：全局局部聚合用于获取实体嵌入，冲突感知伪标记用于对齐增强。两个部分交替迭代直至收敛。

- (2): 为了充分利用实体间的关系结构，该论文对每个实体进行两个级别的邻居聚合，即全局级别的关系聚合和本地级别的实体聚合。全局级别的聚合包括邻居连边的特征向量的拼接和一个非线性转换。本地级别的聚合采用两层GCN和highwaygate策略实现，从而避免了过度平滑化。

- (3): 论文采用关系邻域匹配来纠正嵌入式距离，解决了嵌入式伪标记方法中的误差问题。针对实体嵌入中的对齐冲突问题，采用基于最优输运的对齐方法，通过对未对齐实体之间的传输计划进行优化，从而实现了有效的对齐增强。该方法在多个基准数据集上进行了实验，并在有无先验对齐种子的情况下，均取得了优于现有最先进方法的结果。





8. Conclusion:

- (1): 本论文主要是针对知识图谱实体对齐中存在的冲突问题提出了一种基于最优输运的冲突感知伪标记模型，以提高实体对齐效果。该模型的创新点在于结合OT模型进行对齐增强，显著提高了实体对齐的精度。

- (2): 创新点: 本论文提出了一种新的实体对齐增强方法，利用了最优输运模型对实体进行伪标记，缓解了对齐冲突问题。性能：该方法在多个基准数据集上进行了实验，并在有无先验对齐种子的情况下，均取得了优于现有最先进方法的结果。工作量：论文设计了全局局部聚合的图卷积方法用于学习表达性的实体嵌入，在保证实验效果的同时，工作量适中。但该方法仍存在着一些局限性，例如无法很好地处理实体关系层次结构和新增实体匹配问题。




