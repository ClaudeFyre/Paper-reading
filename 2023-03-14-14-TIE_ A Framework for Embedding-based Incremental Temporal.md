## Paper:1




1. Title: TIE: A Framework for Embedding-based Incremental Temporal

2. Authors: Yixin Cao, Xiangnan He, Xiwei Xu, Qiang Liu, Yongliang Lu, Tat-Seng Chua

3. Affiliation: 华南理工大学

4. Keywords: Knowledge graph, Temporal knowledge graph, Temporal knowledge graph completion, Graph neural network

5. Urls: arXiv:2104.08419v3 [cs.AI] 9 May 2021

6. Summary:
- (1): 该文章的研究背景是知识图谱中蕴含的时间信息在知识的表示和推理中的应用。
- (2): 该文章总结了两种解决时态知识图谱完成的方法，即基于时间不变表示方法和时空卷积神经网络方法。然而这两类方法在推断高动态度信息时，时间表示能力和空间结构建模能力相对欠缺。因此，本文提出一种新颖的 TKG 完成方法：TIE，结合了增量式时间嵌入和时空图神经网络，使得模型能够同时处理低和高动态度的知识推断。
- (3): 本文提出的 TIE 方法主要包含两部分：将事实框架转化为TIE记录以及增量式时间嵌入，其中将事实转化为TIE记录允许模型同时处理时序信息和非时序信息，而采用增量式时间嵌入则允许模型快速学习新产生的事实。
- (4): 该方法在多个数据集上进行了实验，包括 KINSHIP, UMLS, ICEWS18 以及了神经问答数据集 MetaQA-Time，结果表明 TIE 方法在不同的数据集上均达到了最先进的结果，并且具有较高的空间效率和时间效率。





8. Conclusion:

- (1): 本研究的意义在于提出了一种能够同时处理低和高动态度的知识推断的 TKG 完成方法 TIE，将增量式时间嵌入与时空图神经网络相结合，使得模型在表示和推理时蕴含的时间信息能更好地被利用。
           
- (2): 创新点：本文提出的 TIE 方法能够同时处理低和高动态度的知识推断，在各个数据集上均取得了最先进的结果。性能：该方法具有高的时间和空间效率，在实验中表现出强大的推理和表示能力。工作负载：该方法在训练时使用的训练数据规模较小，训练时间更为高效。




