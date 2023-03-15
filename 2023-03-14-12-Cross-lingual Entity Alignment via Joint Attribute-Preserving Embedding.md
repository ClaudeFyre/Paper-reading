## Paper:24




1. Title: Cross-lingual Entity Alignment via Joint Attribute-Preserving Embedding (基于联合属性保全嵌入的跨语言实体对齐)


2. Authors: Xin Luna Dong, Evgeniy Gabrilovich, Geremy Heitz, Wilko Horn, Ni Lao, Kevin Murphy, Thomas Strohmann, Shaohua Sun, Wei Zhang


3. Affiliation: Xin Luna Dong属于谷歌, 其余作者无明确所属机构


4. Keywords: Entity alignment, knowledge base, cross-lingual, embedding


5. URLs: paper link: http://arxiv.org/abs/1708.05045v2, Github: None


6. Summary:

- (1):文章研究了跨语言的实体对齐问题在知识库上的应用。

- (2):以往的跨语言实体对齐方法依靠机器翻译，但这种方法通常受到翻译质量的影响。最新的基于嵌入的技术不需要机器翻译，但大量属性仍然没被很好的处理。文章提出了一种联合的属性保全嵌入模型，用于跨语言实体对齐。此方法将两个知识库的结构统一嵌入到一个向量空间中，并利用知识库中的属性相关性对其进行完善。 

- (3):文章提出了跨语言实体对齐的联合属性保全嵌入模型（Joint Attribute-Preserving Embedding for Cross-lingual Entity Alignment），并进一步进行了实体和属性的联合嵌入实验。 

- (4):实验结果表明，与其他跨语言实体对齐方法相比，此方法在真实数据集上都有显著提升，并可与使用机器翻译的方法相互补充。
7. Methods: 

- (1): 本文提出了一种跨语言实体对齐的联合属性保全嵌入模型，用于将来自两个不同语言的实体对齐到同一空间中。该模型包括两个步骤：首先使用多层感知机（Multi-Layer Perceptron，MLP）将两个知识库的结构嵌入到一个向量空间中，然后使用属性约束将两个向量空间结合起来。

- (2): 该模型还使用了一种属性对齐机制，用于对齐来自不同语言的相似属性，以实现更准确的跨语言实体对齐。此外，还采用了一种优化方法，通过迭代更新实体和属性的嵌入向量，提高了模型的性能。

- (3): 在实验中，本文将提出的模型与现有的跨语言实体对齐模型进行了比较，结果表明其在真实数据集上的表现要优于其他方法。同时，作者还探究了不同参数对模型性能的影响，找到了最优的参数组合。





8. Conclusion:

- (1): 本文研究了基于联合属性保全嵌入的跨语言实体对齐方法，通过将来自两个语言的实体嵌入同一向量空间中，进一步利用属性相关性实现更准确的对齐。实验结果表明此方法在真实数据集上胜过其他跨语言实体对齐方法，具有重要的实际应用价值。

- (2): 创新点：文章提出了一种联合属性保全嵌入模型，不需要机器翻译，用于跨语言实体对齐，并采用了属性对齐机制。性能：本文提出的方法在真实数据集上具有显著优势，可与使用机器翻译的方法相互补充。工作量：在实验中，为找到最优参数组合，作者进行了大量的参数优化工作。




