## Paper:40




1. Title: Multi-modal Entity Alignment in Hyperbolic Space (多模态超几何空间下实体对齐)
2. Authors: Jiemin Chen, Qi Zhu, Jian Tang, Yuxiang Ren, Congying Xia, Yuan Fang, Haitao Zheng
3. Affiliation: Jiemin Chen, Tsinghua University (清华大学)
4. Keywords: Multi-modal Knowledge Graph, Entity Alignment, Hyperbolic Space, Graph Convolutional Networks, Image Embedding
5. Urls: http://arxiv.org/abs/2106.03619v1, Github: None
6. Summary:
   - (1):本文研究背景是多模态知识图谱的整合和实体对齐问题。
   - (2):现有的实体对齐方法大多在欧几里得空间中进行，会导致知识图谱的分层结构失真。同时，对于图像信息的利用也不够充分。本文提出一种基于超几何空间的多模态实体对齐方法（HMEA），利用超几何图卷积网络学习实体结构表示，并使用更先进的图像嵌入模型生成超几何空间中的图像嵌入，最终结合图像信息和知识图谱结构信息获得实体对齐结果。本文方法的动机合理。
   - (3):本文方法采用超几何空间表示实体，使用超几何图卷积网络学习实体结构表示，将图像信息映射到超几何空间中，并最终将图像信息和知识图谱结构信息在超几何空间中结合实现实体对齐。
   - (4):本文方法在多模态知识图谱实体对齐任务上表现出了明显提升，Extensive experiments and ablation studies(大量的实验和消融研究)证明了我们提出的方法和组件的有效性。
7. Methods: 

- (1): 该方法在超几何空间下实现多模态知识图谱的实体对齐，利用超几何图卷积网络学习实体结构表示，并将图像信息映射到超几何空间中，最终结合图像信息和知识图谱结构信息获得实体对齐结果。

- (2): 针对实体对齐问题，本文方法采用多模态信息融合策略，通过超参数β(balance hyper-parameter)来表征结构信息和视觉信息的重要性，将二者结合起来进行实体对齐。

- (3): 本文方法实验采用了公开数据集（FreeBase, DBpedia, YAGO15K），采用 Hits@k作为评价指标，通过与其他基线方法的对比展示了方法的有效性。

- (4): 为了让训练的嵌入空间受限于超曲面而不是 Euclidean 空间，本文方法采用 margin-based ranking loss ，最小化正样本之间的距离，并尽可能增大负样本之间的距离。

- (5): 该方法的构建分三个部分：结构表示学习，视觉表示学习和多模态融合。其中结构表示学习采用 HGCN，在 hyperboloid manifold 上进行 embedding ；视觉表示学习利用 densenet 模型，将图片映射到超几何空间中；融合两部分信息后，利用预先定义的超几何距离度量来判断实体是否匹配。





8. Conclusion: 

- (1): 本文提出了一种基于超几何空间的多模态实体对齐方法，解决了多模态知识图谱整合和实体对齐的问题。该方法在知识图谱分层结构和图像信息的整合方面进行了创新。

- (2): 创新点：本文提出了基于超几何空间的多模态实体对齐方法，充分利用图像信息和知识图谱分层结构，具有较大的创新性。性能：本文方法在多模态实体对齐任务上，表现出了较好的成果，与其他基线方法相比，取得了更好的效果。工作量：本文方法实现较为复杂，需要采用超几何图卷积网络、图像嵌入模型等技术，实现多模态信息的整合。




