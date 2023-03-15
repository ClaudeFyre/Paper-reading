## Paper:42






1. Title: Multilingual Knowledge Graph Completion with Joint Relation and Entity Alignment (多语言知识图谱补全与关系及实体对齐)

2. Authors: Moumita Bhattacharya, Dongyeop Kang, Anirban Roy, Gerhard Weikum

3. Affiliation: 萨尔布吕肯马克斯·普朗克计算机科学研究所（Max Planck Institute for Informatics）

4. Keywords: Knowledge Graph Completion, Multilingual, Entity Alignment, Relation Alignment, Soft Asymmetric Overlap, Joint Training

5. Urls: https://arxiv.org/abs/2104.08804v1, Github:None 

6. Summary: 

- (1):本文的研究背景是知识图谱补全，旨在将补全在不完整知识图谱中缺失的事实，同时，不同语言的知识图谱之间语义的不同以及实体和关系的不同标识符会导致信息匹配任务复杂。 

- (2):目前的方法只能针对一个语言一次处理，不具有扩展性，不同语言下的 KG均只能独立地进行补全;ID标识符的不一致性也导致匹配困难。文中提出了一个多语言联合模型，共同进行知识图谱完成、实体对齐和关系对齐，通过联合训练将它们联系起来，解决了语言和实体关系的匹配问题，提升了补全和匹配的效果。

- (3):文章提出了一个称为ALIGNKGC的通过种子实体和关系对齐来联合优化补全、实体对齐和关系对齐损失的多任务系统，其核心是基于每种关系的（主题，客体）集项签名的嵌入式软不对称重叠，采用端到端训练协议进行训练。

- (4):实验证明，与单个 KG系统相比，ALIGNKGC在所有任务上都取得了良好的成效，单个 KG中补全模型相比，ALIGNKGC在 10-32 MRR的不同语言数据集上分别提升了多项性能进步，实验表明对于 EA 和 RA， ALIGNKGC取得了相对较强的性能提升，验证了联合训练对 EA 和 RA 任务的价值。





8. Conclusion:

- (1): 本文提出了一个多语言联合模型，通过联合训练完成知识图谱的补全、实体对齐和关系对齐，并解决了不同语言和实体标识符之间的匹配问题，对于提高知识图谱的准确性和扩展性具有重要意义。

- (2): 创新点：ALIGNKGC将关系对齐与知识图谱补全和实体对齐相结合，有效解决了多语言KG中的信息匹配问题。性能：ALIGNKGC在各项任务上均表现优异，在十几个不同语言的数据集上均取得了对单个KG模型相当甚至更高的结果。工作量：ALIGKGC需要对多语言KG进行预处理和嵌入学习，工作量相当大，但在提高效果方面是值得付出的。






