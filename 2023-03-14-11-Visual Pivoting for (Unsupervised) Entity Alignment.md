## Paper:20




1. Title: Visual Pivoting for (Unsupervised) Entity Alignment (基于视觉枢轴的实体对齐方法)

2. Authors: Tong Chen, Weijie Liu, Xiao Liu, Chenyan Xiong, Xiaodong Liu, Dawn Song, Jiawei Han

3. Affiliation: 伊利诺伊大学厄巴纳香槟分校计算机科学系

4. Keywords: Knowledge Graph, Entity Alignment, Visual Modality, Unsupervised Learning, Multi-modal Embedding

5. Url: Paper: http://arxiv.org/abs/2009.13603v2, Github: https://github.com/cambridgeltl/eva

6. Summary: 
- (1):本文的研究背景是知识图谱实体对齐，旨在将来自不同通路或语言的知识图谱中的实体对齐，以获得更全面、更全面的知识。
- (2):过去的方法包括基于同构性的方法、基于嵌入的方法和基于图神经网络的方法等等，它们的问题在于很难获得足够的跨图谱种子对齐。为此，本文提出了一种利用视觉语义知识构建实体嵌入的方法，通过视觉相似性引入一个中间自动生成的种子字典，从而实现完全无监督的实体对齐。本文提出的方法在两个标准的数据集DBP15k和DWY15k上都获得了最先进的表现，同时发现图谱中的图像对于对齐丰富实体是特别有用的。
- (3):本文提出了一种名为EVA（Entity Visual Alignment）的方法，它结合了视觉、关系、结构和属性信息对不同的知识图谱中的实体进行对齐。通过可学习的注意力加权方案，可以帮助对齐模型决定每种模态的重要性，并且提供每种模态的贡献的解释。该模型可在以前方法中使用少量的种子对齐标签（半监督设置），或者仅使用一组自动感应的视觉中心点（无监督设置）进行训练，均可进行迭代学习来扩大训练种子的数量。该模型在两个跨语言和单语言的EA基准测试数据集上均获得了最好的表现。
- (4):EVA方法提供了三重贡献：（i）首次研究在KG中使用图像作为实体表示部分进行EA，实现了最先进的表现；（ii）通过利用视觉相似性提出了一种完全非监督的EA设置，避免了对以前方法中通常需要的任何黄金标签的依赖；（iii）我们通过解释每种模态的贡献并进行彻底的错误分析来提供可解释性。


7. Methods:

- (1): 本文提出了一种视觉枢轴的实体对齐方法（EVA），旨在实现不同知识图谱中实体的无监督对齐，以获得更全面和更准确的知识。该方法结合了不同模态的信息，包括视觉、关系、结构和属性信息，并通过学习注意力权重来决定模态的重要性。
 
- (2): EVA方法采用了多模态嵌入学习过程，将两个知识图谱转换为一个共享的低维向量空间，并通过图卷积网络（GCN）学习了不同嵌入的表示，通过可训练的加权方案来融合多模态信息。然后，通过Neighbourhood Component Analysis（NCA）和迭代学习来对齐对应实体，并实现对未标记数据的对齐。
 
- (3): 该方法还提出了一种自动感应的视觉字典，可通过对视觉嵌入进行相似性的计算自动为多图谱中的实体生成种子标签，从而实现完全的无监督学习。该方法在两个基准数据集（DBP15k和DWY15k）上都获得了最先进的表现，并提供了可解释性。





8. Conclusion: 

- (1): 本篇文章提出的EVA方法引入图谱实体的视觉相似性，并利用可学习的注意力权重对不同模态信息进行加权融合以实现实体对齐。该方法提出了一种完全无监督的实体对齐方法，并在两个标准数据集上获得了最先进的表现，提供了可解释性。该研究表明视觉感知是学习实体表示和关联知识的重要元素。

- (2): 创新点：EVA方法结合了视觉、关系、结构和属性信息，并提出了一种利用视觉相似性生成种子字典，实现完全无监督的实体对齐。性能：该方法在两个标准数据集上均获得了最先进的表现，并提供了可解释性。工作量：实验结果表明，EVA方法的训练时间比以前的方法更短，同时需要大量存储，但存储需求比最近的对齐方法少。



