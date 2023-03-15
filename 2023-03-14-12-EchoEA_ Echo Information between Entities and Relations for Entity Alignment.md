## Paper:44






1. Title: EchoEA: Echo Information between Entities and Relations for Entity Alignment（EchoEA：用于实体对齐的实体和关系之间的回声信息）

2. Authors: Zhongqing Wang, Yuting Wu, Wei Wang, Bolin Ding, Peng Zhang, Wei Zhang, Hongbin Zhou

3. Affiliation: 上海交通大学 (Shanghai Jiao Tong University)

4. Keywords: entity alignment, knowledge graph, graph neural network, self-attention, bootstrapping

5. Urls: Paper: http://arxiv.org/abs/2107.03054v2, Github：None

6. Summary:

- (1): 本文研究背景是实体对齐（EA）在多源知识图谱（KGs）自动集成中的作用越来越重要，当前GNN编码器方法还存在深度限制和半监督Bootstrapping质量低的问题，为此提出了EchoEA实体对齐的创新方法以及解决半监督过程中采用的attribute-combined bi-directional global-filtered策略来生成高质量的训练数据。 

- (2): 过去的EA方法包括Translation-based models、rotating models、polar coordinate models、bilinear models、hyperbolic geometry models、Convolution-based models、Capsule-based models等，但是传统的KGE方法在EA任务中表现不如GNN的方法，而GNN-based方法在自监督Bootstrapping时的质量较低，且2层的GCN-Align、GGNN-Align表现优于多层的方法。为了提高GNN的性能和质量，本文提出了EchoEA方法，用4级self-attention机制来将实体信息传播到关系并反响到实体，同时使用了attribute-combined bi-directional global-filtered策略来生成bootstrapping数据。 

- (3): 本文的研究方法是将self-attenton与GCN联合，EchoEA在这两个机制的基础上提出了包括元素attenton在内的四级self-attention-memory结构，通过加入attribute-combined bi-directional global-filtered策略来解决bootstrapping中数据量大小和质量的问题。 

- (4): 本文基于三个真实的跨语言数据集进行了实验研究，结果表明所提出的EchoEA方法在hits@1上的平均稳定性已达到96%左右，大大优于现有的GNN-based方法，同时具备了泛化性和可转移性。
7. Methods:

- (1): 本文提出了EchoEA实体对齐方法，该方法涉及到四级self-attention-memory结构和attribute-combined bi-directional global-filtered策略的使用。其中，四级self-attention-memory机制涉及元素attention和关系attention的使用，可将实体信息传播到关系并反响到实体。attribute-combined bi-directional global-filtered策略旨在生成足够的高质量训练数据。

- (2): EchoEA使用的四级self-attention-memory结构可有效捕捉实体、关系和全局信息之间的联系，而此机制中的元素attention和关系attention可更好地调整实体和关系之间的注意力权重。

- (3): EchoEA采用attribute-combined bi-directional global-filtered策略，利用多个跨语言词典和数据图进行半监督bootstrapping，提高了数据的质量和常规性，并缓解了传统意义下的数据不平衡问题。

- (4): 在实验过程中，本文针对三个跨语言实体对齐数据集进行测试，结果表明EchoEA方法优于其他GNN-based方法，表现稳定，具有很好的泛化和可迁移性。





8. Conclusion:

- (1): 本文提出了一种新的跨语言实体对齐框架EchoEA，并在实现自我监督时提出了Attribute-combined Bi-directional Global-filtered策略以生成高质量的训练数据。EchoEA方法利用四级self-attention-memory结构将实体信息传播到关系并反响到实体，以及利用了多种跨语言词典和数据集进行半监督bootstrapping。该研究的意义在于提高了多源知识图谱自动集成中实体对齐的表现，提高了迁移性能。

- (2): 创新点：本文提出了EchoEA实体对齐方法，包括四级self-attention-memory结构和Attribute-combined Bi-directional Global-filtered策略的使用。性能：实验结果表明，EchoEA方法在三个真实跨语言数据集上的hits@1平均稳定性达到96%，远高于其他GNN-based方法，具有很好的泛化性和可迁移性。工作量：本文实现了一个更深的实体编码器Echo，并提出了半监督bootstrapping数据的生成方法，因此工作量相对较大，但提高了跨语言实体对齐的准确性和效率。




