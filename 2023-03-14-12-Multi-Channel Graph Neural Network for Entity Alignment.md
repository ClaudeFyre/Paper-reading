## Paper:69




1. Title: Multi-Channel Graph Neural Network for Entity Alignment (多通道图神经网络用于实体对齐)
                
                2. Authors: Hongbin Ye, Zhiqing Sun, Chi Wang, Tong Ruan, Wei Zhang, Xuemin Lin
                
                3. Affiliation: 香港中文大学(CUHK)
                 
                4. Keywords: knowledge graph, entity alignment, graph neural network, multi-channel, cross-lingual
                
                5. Urls: 
                   - Paper: http://arxiv.org/abs/1908.09898v1
                   - Github: None 
                    
                6. Summary: 

                    - (1):本文研究的问题是知识图谱中实体对齐问题。由于不同的知识图谱结构异构性，学习它们的向量嵌入并将它们对齐是很具挑战的。
 
                    - (2
7. Methods:

- (1): 本研究提出了一种新的多通道图神经网络（MuGNN）方法用于知识图谱中的跨语言实体对齐问题。该方法包括两个通道，一个是针对知识图谱的自我注意力通道（KG Self-Attention Channel），另一个是针对跨语言信息的交叉知识图谱注意力通道（Cross-KG Attention Channel）。此外，该方法还引入一个基于预先提取的规则的一致性完成和修剪方法（Rule Transfer）。MuGNN综合利用公共部分知识和异构信息，从而弥补不同知识图谱之间结构的差异，实现跨语言实体对齐。

- (2): 此外，本研究比较了MuGNN与四种已有的跨语言实体对齐方法（MTransE，JAPE，GCN-Align，AlignEA）的表现。其中，实验数据集包括DBPZH-EN，DBPJA-EN，DBPFR-EN，DBP-WD和DBP-YG等。评估指标包括Hit@N和平均倒数排名（MRR）。实验表明，MuGNN相比于其他方法具有更好的性能表现，特别是在DBP-YG这个大规模实验数据集中，平均性能提高了8%。这是因为MuGNN采用了AMIE+规则挖掘方法，能够显式地完成两个知识图谱并完成规则迁移，从而更好地利用种子对齐信息。

- (3): 最后，本研究还进行了模型敏感度分析和组件分析。具体而言，作者通过移除两个通道或移除Ruule Transfer等措施来探究各个组件对于性能提升的贡献。分析结果表明，两个通道和规则迁移对于MuGNN的性能提升贡献较大。同时，本研究还探究了种子对齐数量对于实体对齐结果的影响，发现GNN-based方法在种子对齐数量较少（10%）时表现更好，而随着种子对齐数量的增多（50%），更趋向于表现较差，而基于翻译的方法随着种子对齐数量的增多表现逐渐提升。





8. Conclusion:

- (1): 本文的意义在于提出了一种新的多通道图神经网络方法用于知识图谱中的跨语言实体对齐问题。该方法充分综合利用了知识图谱结构的异构性以及跨语言信息，实现了不同知识图谱之间的对齐，对于实现知识图谱的交互和共享具有重要意义。

- (2): 创新点：MuGNN采用了两个新的通道针对不同信息，同时引入预先提取的规则的一致性完成和修剪方法（Rule Transfer）。性能：实验结果表明，MuGNN相比于其他跨语言实体对齐方法具有更好的性能表现，特别是在大规模实验数据集DBP-YG中，平均性能提高了8%。工作量：本文的数据集来源比较广泛，实验设置合理，同时还进行了系统的敏感度分析和组件分析，对MuGNN的性能提升作出了说明，但对于一些具体参数的设置介绍不够详细，可能需要在后续研究中进一步探究。




