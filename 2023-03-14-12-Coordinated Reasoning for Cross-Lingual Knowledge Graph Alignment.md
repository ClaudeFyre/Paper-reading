## Paper:37







1. Title: Coordinated Reasoning for Cross-Lingual Knowledge Graph Alignment (跨语言知识图谱对齐的协调推理)
 
2. Authors: Lianli Gao, Xiang Deng, Wanxiang Che, Yong Liu

3. Affiliation: Lianli Gao- State Key Laboratory on Intelligent Technology and Systems, Department of Computer Science and Technology, Tsinghua University, Beijing, China (中国清华大学计算机科学与技术系智能技术与系统国家重点实验室); Xiang Deng, Wanxiang Che, Yong Liu- MOE Key Lab of Computational Linguistics, School of EECS, Peking University, Beijing, China (中国北京大学电子学院计算机所计算语言学教育部重点实验室)

4. Keywords: knowledge graph, cross-lingual alignment, coordination reasoning, entity alignment, graph matching network

5. URLs: Paper: http://arxiv.org/abs/2001.08728v1; Github: None

6. Summary:

- (1): 本文研究跨语言知识图谱对齐的协调推理问题。知识图谱(KGs) 是表示实体及其关系的全球事实信息的图形化格式，已经在许多自然语言处理应用程序中成功应用，如问答和关系提取。但是KGs产生于不同语言，而各个语言的KGs共享很多相同的事实，也提供了其他KGs都未涵盖的不同信息，因此建立不同语言的KGs之间的交叉语言对齐是非常有益的。
 
- (2): 现有entity alignment方法主要在编码知识图的选择上有所变化，但通常使用相同的解码方法，即独立地为每个源实体选择最佳匹配项。这种解码方法不仅可能导致"一对多"问题，而且忽略了这个任务的协调性，即每个对齐决策可能高度相关于其他决策。本文引入了两种协调推理方法，即Easy-to-Hard解码策略和联合实体对齐算法。具体而言，Easy-to-Hard策略首先从预测结果中检索模型置信度的对齐结果，然后将其作为附加知识来解决剩余的模型不确定对齐问题。为此，我们进一步提出了基于当前最先进基线的增强对齐模型。此外，为了解决“一对多”问题，我们建议联合预测实体对齐，使一对一约束可以自然地纳入对齐预测。实验结果表明，我们的模型实现了最先进的性能，而我们的推理方法也可以显著改进现有基线方法。
 
- (3): 本文提出两种协调推理方法——Easy-to-Hard解码策略和联合实体对齐算法。Easy-to-Hard策略关注的是从预测结果中获得模型置信度的对齐结果，联合实体对齐算法解决了一对多问题，使一对一约束可以自然地纳入对齐预测中。
 
- (4): 本文的实验任务是跨语言知识图谱对齐。实验结果表明，所提出的模型显著优于现有基线方法，Easy-to-Hard策略、联合实体对齐算法等协调推理方法也可以显著改善现有基线方法。因此，所提出的方法有效地解决了现有实体对齐方法中常见的漏解决一对多问题的问题。
7. Methods:

- (1): 本文针对跨语言知识图谱对齐任务，提出了两种协调推理方法。Easy-to-Hard解码策略首先从预测结果中检索置信度高的对齐结果，然后将其作为附加知识解决剩余的未确定对齐问题。为此，对齐模型被增强，并提出了基于当前最先进基线的增强对齐模型。联合实体对齐算法建议联合预测实体对齐，使一对一约束可以自然地纳入对齐预测。

- (2): 实验中，我们检索出前10个实体对齐，将它们的分数归一化为概率，并在其上执行所提出的协调推理方法。对于Easy-to-Hard解码方法，设置α为0.75，K为20。对于联合实体对齐算法，设置τ为0.10。通过随机选择最多两个标准的对齐，模拟Easy-alignments的数据，训练增强的对齐模型。

- (3): 实验结果表明，我们的模型实现了最先进的性能，而我们的推理方法也可以显著改进现有基线方法。本文提出的两种协调推理方法可以有效地解决跨语言知识图谱对齐中经常遇到的“一对多”问题。





8. Conclusion:

- (1): 本文的意义在于提出了两种协调推理方法，以解决跨语言知识图谱对齐中的经典问题。所提出的Easy-to-Hard解码策略和联合实体对齐算法可以有效降低“一对多”问题的影响，优化跨语言知识图谱的对齐。此外，本文所提出的基于当前最先进基线的增强对齐模型可以作为实体对齐任务的benchmark，未来的研究可以在此基础上进一步探索。

- (2): 创新点：本文提出了两种协调推理方法，解决了entity alignment任务中的常见问题；性能：所提出的模型实现了最先进的性能，且能够改进现有基线方法的性能；工作量：本文提出的方法实现相对简单，但实验中需要进行的实体对齐任务较为耗时。




