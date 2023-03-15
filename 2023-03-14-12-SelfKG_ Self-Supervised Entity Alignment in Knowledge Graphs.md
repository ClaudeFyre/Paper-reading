## Paper:22




1. Title: SelfKG: Self-Supervised Entity Alignment in Knowledge Graphs (无监督下的知识图谱实体对齐：SelfKG)


                 2. Authors: Xinyi Liu, Haoxu Hong, Xiangnan Wang, Zhirong Chen, Evgeny Kharlamov, Yong Dong, Jie Tang


                 3. Affiliation: 西安交通大学 (Xi'an Jiaotong University)


                 4. Keywords: Self-supervised learning, Knowledge Graph, Entity alignment, Relative similarity metric, Self-negative sampling
                    
                 
                 5. Urls: Paper: http://arxiv.org/abs/2203.01044v1, Github: https://github.com/THUDM/SelfKG


                 6. Summary: 


                    - (1):本文围绕知识图谱实体对齐问题展开研究，探讨了无监督下的实体对齐技术。

                    - (2):文章指出传统实体对齐方法存在需要大量标注数据和标注数据可能存在偏差等问题。为解决这些问题，本文提出了一种基于自监督学习策略的SelfKG框架。

                    - (3):SelfKG框架通过引入相对相似度指标、自定义负采样策略和多重负采样技术等方法实现无监督下的实体对齐。

                    - (4):本文在DWY100K和DBP15K等数据集上对SelfKG算法进行评测，结果表明SelfKG算法无需标注数据就可以实现与有监督方法相当的实体对齐性能，证明了自监督学习在知识图谱实体对齐问题中的潜力与优越性。
7. Methods: 

- (1): SelfKG框架采用无监督学习策略实现知识图谱实体对齐。该框架基于相对相似度指标和自定义负采样策略，在无需标注数据的情况下进行实体对齐。

- (2): 相对相似度指标是自监督学习的核心。文章提出了一种基于相对相似度指标的 NCE 损失函数， 该函数不需要标注数据即可指导模型学习。对于正样本，该函数的对齐项"pulling" 使正样本更加接近。对于负样本，函数的相似度项"pushing" 使模型将与对齐实体相关的不同实体推得更远。

- (3): 为避免采样冲突，SelfKG框架引入了自定义负采样策略。选择从同一个知识图谱中采样耦合负样本排除重复。通过扩展MoCo技术并维护负样本队列，实现大规模负样本采样并降低计算复杂度。

- (4):SelfKG框架在DWY100K和DBP15K等数据集上进行实验验证，结果表明其实





8. Conclusion: 

- (1): 本篇文章在知识图谱实体对齐问题中，探究了无监督方法下实体对齐的可行性及其实现方法。该研究意义重大，能够解决传统实体对齐方法需要大量标注数据和数据偏差等问题。
                     
- (2): 创新点：文章提出了基于相对相似度指标和自定义负采样策略的SelfKG框架，实现无监督下实体对齐。性能：在DWY100K和DBP15K等数据集上对SelfKG进行评测，结果表明SelfKG无需标注数据就可以实现与有监督方法相当的实体对齐性能。工作量：文章对自定义负采样策略进行改进，通过扩展MoCo技术维护负样本队列，实现大规模负样本采样，同时减小计算复杂度。




