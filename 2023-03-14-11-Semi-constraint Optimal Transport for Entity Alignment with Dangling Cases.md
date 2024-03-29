## Paper:11




1. Title: Semi-constraint Optimal Transport for Entity Alignment with Dangling Cases (具有悬挂情况的实体对齐的半约束最优传输)

2. Authors: Xiaoling Wu, Shiren Ye, Zhi-Jie Wang, Jiangtao Feng, Min Yang, Qiang Zhang, Xiaofei Guo

3. Affiliation: 华南理工大学 (South China University of Technology)

4. Keywords: entity alignment, dangling entities, optimal transport, knowledge graphs, contrastive metric learning

5. Urls: http://arxiv.org/abs/2203.05744v3, Github: None

6. Summary: 

- (1): 本文主要研究的是知识图谱中的实体对齐问题，介绍了解决悬挂实体对齐问题的一种无监督方法。

- (2): 以往的实体对齐方法主要基于嵌入式对齐，即学习实体的表示向量，并在表示空间中找到最相似的实体对齐，这种方法存在假设每个实体都存在对应实体的缺点。此外，在不同的知识图谱中，经常存在无法找到对应实体的悬挂实体，这种情况限制了实体对齐方法的性能。本文提出了一种名为Semi-constraint Optimal Transport for Entity Alignment in Dangling cases (SoTead)的无监督方法，该方法使用对齐实体之间的最优传输问题来建模两个知识图谱之间的实体对齐。首先，基于预训练词嵌入向量，我们建立了伪实体对。然后，我们进行对比度度量学习，以获取每个实体对之间的传输成本。最后，我们为每个知识图谱介绍一个虚拟实体来“对齐”另一个知识图谱中的悬挂实体，从而放松优化约束，并导致半约束最优传输。与现有方法相比，SoTead的性能更好。

- (3): 本文的主要贡献是提出了一种新的实体对齐方法SoTead。该方法使用对齐实体之间的最优传输问题建模两个知识图谱之间的实体对齐，本文还提出了一个虚拟实体的概念来对齐不匹配实体。此外，为了度量每个实体对之间的传输成本，我们使用了对比度度量学习。

- (4): 本文提出的SoTead方法在常用的实体对齐数据集上超越了现有方法，并在新构建的医学跨语言知识图谱数据集MedED上也取得了同等的优异性能。此外，我们还展示了传输成本的可视化结果，这部分结果进一步说明了我们提出的SoTead方法具有优越的性能。
7. Methods:

- (1): 本文提出了一种半约束最优传输的方法用于解决知识图谱中的实体对齐问题，该方法被命名为Semi-constraint Optimal Transport for Entity Alignment in Dangling cases (SoTead)。该方法使用对齐实体之间的最优传输问题来建模两个知识图谱之间的实体对齐，通过引入虚拟实体来放松优化约束并导致半约束最优传输。

- (2): 为了实现对齐实体之间的传输成本的度量，本文使用了对比度度量学习。首先，基于预训练词嵌入向量，我们建立了伪实体对；然后，我们进行对比度度量学习，以获取每个实体对之间的传输成本；最后，我们为每个知识图谱介绍了一个虚拟实体来对齐不匹配实体。

- (3): 为了解决在不同知识图谱中存在无法找到对应实体的悬挂实体的问题，我们将两个知识图谱中的悬挂实体通过虚拟实体对齐。此外，我们使用了两个超参数α和β来作为虚拟实体和真实实体之间的跨知识图谱距离，以实现半约束最优传输。我们还提出了一种全局引导的优化方法，以利用所有实体的信息来指导最优传输的学习。

- (4): 为了验证所提出的SoTead方法的性能，我们在常用的实体对齐数据集上进行了实验，并在新构建的医学跨语言知识图谱数据集MedED上也对其进行了测试。此外，我们使用传输成本的可视化结果来进一步说明SoTead方法具有优越的性能。





8. Conclusion:

- (1): 本文提出了一个新的半约束最优传输方法SoTead，用于解决知识图谱中的实体对齐和悬挂实体检测问题。本文具有很高的实用价值和研究意义，对知识图谱处理具有广泛的应用前景。

- (2): 创新点：本文提出了一种新颖的对齐方法SoTead，不仅可以对齐实体，还可以检测悬挂实体。性能：本文的实验结果表明，所提出的SoTead方法在常用的数据集上超过了现有方法，并在新构建的医学跨语言知识图谱数据集MedED上也取得了同等的优异性能。工作量：本文的工作量较大，包括对比度度量学习、虚拟实体引入、超参数α和β的设置等研究内容。但是，通过不断的实验，最终得到的结果非常令人满意。




