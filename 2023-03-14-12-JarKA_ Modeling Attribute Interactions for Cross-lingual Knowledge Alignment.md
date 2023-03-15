## Paper:49




 
1. Title: JarKA: Modeling Attribute Interactions for Cross-lingual Knowledge Alignment (JarKA: 建模属性相互作用，实现跨语言知识对齐)

2. Authors: Chen Xu, Lingfei Wu, Chengkai Li, Mohamed M. Hassan, Jiaming Shen, Ziwei Ji

3. Affiliation: Chen Xu (University of Texas at Arlington), Lingfei Wu (University of Texas at Arlington), Chengkai Li (University of Texas at Arlington), Mohamed M. Hassan (University of Texas at Arlington), Jiaming Shen (University of Texas at Arlington), Ziwei Ji (Nanyang Technological University)

4. Keywords: knowledge alignment, cross-lingual, knowledge graph, attribute interactions, entity embeddings

5. Urls: Paper: http://arxiv.org/abs/1910.13105v2; Github: None

6. Summary:

- (1): 本文研究跨语言知识对齐问题，旨在建立一个准确完整的跨语言知识图谱。
 
- (2): 以往研究方法通常只考虑了关系三元组来对齐实体，忽略了实体的属性信息，同时不同知识图谱之间的属性也存在异构性，因此无法精准地嵌入和比较实体的属性信息。本文提出了一种建模实体属性相互作用的方法，通过对实体的属性信息进行交互式建模，来更加准确地进行跨语言知识对齐任务。
 
- (3): 本文提出了一种 JarKA 模型，该模型包括一个基于交互式建模的属性模型和一个基于嵌入的关系模型，并采用一个联合框架将两个模型结合起来，实现跨语言知识对齐任务。
  
- (4): 实验结果表明，与目前的对比方法相比， JarKA 模型具有更好的对齐效果，在提高的对齐精度下，同时也实现了较高的效率，能够较好地支持本文的目标。





8. Conclusion:

- (1): 本文的意义在于，针对跨语言知识对齐任务中存在的实体属性信息不充分、异构性较强等问题，提出了一种新颖的基于交互式建模实体属性相互作用的方法， JarKA 模型。该模型能够实现更准确的跨语言知识对齐，有助于构建更加完整的跨语言知识图谱，为跨语言自然语言处理和知识图谱领域的研究提供了新思路。

- (2): 创新点：本文提出了一种建模实体属性相互作用的方法， JarKA 模型，能够更准确地进行跨语言知识对齐任务。性能：实验结果表明， JarKA 模型具有更好的对齐效果，在提高的对齐精度下，同时也实现了较高的效率。工作量：本文在模型设计和实验验证方面做了大量的工作，但是其模型训练和测试的数据集较小，后续需要进一步扩大数据集的规模和深入验证模型的鲁棒性。




