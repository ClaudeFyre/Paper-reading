## Paper:72




1. Title: Weakly-supervised Knowledge Graph Alignment with Adversarial Learning（弱监督知识图谱对齐的对抗性学习）

2. Authors: Meng Qu, Jian Tang, Jingbo Shang

3. Affiliation: MontreaI Institute for Learning Algorithms (MILA)，University of Montr´eal，Canadian Institute for Advanced Research (CIFAR)

4. Keywords: knowledge graph alignment, weakly-supervised learning, adversarial learning, unsupervised learning, triplets

5. Urls: Paper: http://arxiv.org/abs/1907.03179v1; Github: None

6. Summary:

- (1):  本文的研究背景是不同源或语言的知识图谱对齐。 
- (2):  目前的方法通常需要大量的三元组数据进行训练，然而在许多领域这种大量的数据可能不可用或成本过高。因此，本文提出了一个无监督或弱监督的方法来对齐知识图谱，即不需要或者只需要一些对齐的三元组。本文提出了一种对抗性学习框架，利用最大化不同的知识图谱之间嵌入的互信息的正则化项来减轻学习对齐函数时出现的模式崩塌问题。并可以利用少量的对齐三元组作为指导，无缝地将其与现有的监督方法结合。 目前的方法通常需要大量的三元组数据进行训练，然而在许多领域这种大量的数据可能不可用或成本过高。因此，本文提出了一个无监督或弱监督的方法来对齐知识图谱，即不需要或者只需要一些对齐的三元组。本文提出了一种对抗性学习框架，利用最大化不同的知识图谱之间嵌入的互信息的正则化项来减轻学习对齐函数时出现的模式崩塌问题。并可以利用少量的对齐三元组作为指导，无缝地将其与现有的监督方法结合。 
- (3): 本文提出的无监督框架利用现有的知识图谱嵌入方法（例如TransE），首先将不同知识图谱的实体和关系以低维空间进行表示，然后学习对齐函数pe(et | es)和pr(rt | rs)，将源知识图谱的实体和关系（es和rs）映射到目标图谱中的那些（et和rt）。 
- (4): 在多个数据集上的实验结果表明，本文提出的方法在无监督和弱监督设置下都有效。 性能支持其目标。
7. Methods: 

- (1): 本文提出的方法是一种无监督或弱监督的知识图谱对齐方法。首先，使用现有的知识图谱嵌入方法（例如TransE）将不同知识图谱的实体和关系以低维空间进行表示。然后，学习对齐函数pe(et | es)和pr(rt | rs)，将源知识图谱的实体和关系（es和rs）映射到目标图谱中的那些（et和rt）。
 
- (2): 文中提出了一种对抗性学习框架，利用最大化不同知识图谱之间嵌入的互信息的正则化项，来减轻学习对齐函数时出现的模式崩塌问题。具体来说，对于对齐的三元组和非对齐的三元组，分别设计两个对抗性损失函数，目的是让嵌入分布和对齐函数分布间的差异最大化，以防止学习到相似的嵌入或相同的对齐函数。
 
- (3): 为了进一步提高对齐的质量，本文还引入了一种半监督的策略，在学习对齐函数的同时，利用少量的对齐三元组进行监督学习。这个策略集成了无监督和监督方法的优点，并获得了更好的对齐结果。
 
- (4): 实验结果表明，本文提出的方法在无监督和弱监督设置下都有效。此外，本文在多个数据集上进行了实验，展示了本方法优于其他状态-of-the-art的方法的性能。





8. Conclusion: 

- (1): 本文提出了一种无监督或弱监督的知识图谱对齐方法。之前的方法需要大量数据进行训练，而本文提出的方法不需要或者只需要一些对齐的三元组。通过对抗训练和互信息最大化，我们的方法能够将不同知识图谱中的实体和关系进行对齐。此外，该方法还能够与现有的有监督方法融合，形成一种弱监督的方法，扩大了其适用范围，具有很高的实用意义。
    
- (2): 创新点：本文提出的无监督或弱监督的知识图谱对齐方法是一种以对抗性训练和互信息最大化为基础的方法，不需要大量对齐数据，能够有效处理许多领域的对齐问题，并且能够与现有的有监督方法进行无缝结合。
    
 性能：在多个数据集上的实验结果表明，本文提出的方法在无监督和弱监督设置下，均能取得比其他方法更好的对齐效果。
   
 工作负荷：由于使用了现有的知识图谱嵌入方法（如TransE），本文提出的方法不需要大量的计算资源或时间。并且，本文的方法可以利用少量的对齐三元组进行监督学习，因此很实用。




