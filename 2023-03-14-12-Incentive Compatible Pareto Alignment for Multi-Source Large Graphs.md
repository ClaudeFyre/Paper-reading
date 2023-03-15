## Paper:61






1. Title: Incentive Compatible Pareto Alignment for Multi-Source Large Graphs (多源大规模图形的激励兼容 Pareto 对齐)

2. Authors: Jian Liang, Fangrui Lv, Di Liu, Zehui Dai, Xu Tian, Shuang Li, Fei Wang, Han Li

3. Affiliation: 中国科学技术大学 (University of Science and Technology of China)

4. Keywords: multi-source entity-matching, graph neural network, Pareto front optimization, negative transfer, incentive-compatible mechanism

5. Urls: 
- Paper: http://arxiv.org/abs/2112.02792v1
- Github: None

6. Summary:

- (1): 本文研究的是多源大规模数据中的有效实体匹配模型，针对真实应用的多源数据分布/空间和实体身份没有共享的情况进行放宽，提出了一个放松的多源大规模实体匹配 (RMLE) 问题。难点主要包括如何对齐来自不同数据源的大规模实体以共享信息，以及如何缓解联合学习多源数据中的负转移。为了解决这些挑战，本文提出了一种激励兼容的 Pareto 对齐 (ICPA) 方法，通过 Pareto 前沿优化优化信息共享，然后在优化的对齐基础上缓解负转移。具体来说，Pareto 前沿优化鼓励最小化负转移的下限，并优化何时以及哪些来对齐。
- (2): 过去的方法通常假设多源数据分布/空间和实体标识在数据源之间共享，或者可以获取足够的实体对应关系注释，但在真实应用中这些假设并不一定成立。同时，负转移的问题也是多源数据实体匹配中的一个难点。本文的方法的动机合理，通过 Pareto 前沿优化解决信息共享和负转移兼容问题。
- (3): 本文提出了一个基于图神经网络的方法来解决 RMLE 问题，通过将实体作为节点、匹配关系作为加权边来建模，对于每个数据源，建立一个图。然后使用 graph matching（图匹配）方法来对这些图中的实体进行对齐，以便它们在学习过程中可以共享信息。针对负转移问题，本文提出了激励兼容的 Pareto 对齐机制，以让每个数据源都能够根据自己的真实偏好优化模型，而不必担心其他数据源的表现下降。
- (4): 本文在国际实体图 (IEG) 数据集以及三个真实世界的大规模基准数据集上进行了全面实验评估，同时在一个搜索广告平台上进行了在线A / B测试。评估结果表明，ICPA 方法效果显著。所提出的 Pareto Multi-Task Learning 框架和节点对齐模型在数据集上取得了良好的性能。
7. Methods: 

- (1): 本文提出的方法主要包括三个步骤：
        - Step 1：建立多源数据中的图形，将每个实体作为节点，将不同实体之间的相互关系作为加权边。同时，对于每个数据源，都建立一个对应的图形。
        - Step 2：通过使用图匹配算法对不同数据源中的实体进行对齐，以便它们可以共享信息。
        - Step 3：基于 Pareto 前沿优化，设计激励兼容机制，以达到信息共享和负转移问题的兼容目标。

- (2): 本文中采用的算法





8. Conclusion: 

- (1): 本文提出了多源大规模实体匹配问题的激励兼容 Pareto 对齐方法。针对多源数据中实际应用中存在的分布/空间和实体身份不共享的情况，提出了一个放松的 RMLE 问题。该方法能够解决信息共享和负转移等问题，优化多源数据实体匹配。本文在图神经网络和 Pareto 前沿优化方面进行了有益探索，为多源数据实体匹配问题的研究带来了新的启示。 

- (2): 创新点：本文提出了激励兼容 Pareto 对齐的方法，能够解决多源数据实体匹配中存在的信息共享和负转移问题。相比于传统方法，创新点明显。表现：在 IEH 数据集以及三个真实世界的大规模基准数据集上进行全面实验评估，同时在搜索广告平台上进行了在线 A/B 测试。评估结果表明，ICPA 方法效果显著。工作量：本文提出的方法在论文中给出了详细的推导过程和实现细节，实验评估结果得到了充分验证，因此工作量适中。



