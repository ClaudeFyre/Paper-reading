## Paper:7




1. Title: Ensemble Semi-supervised Entity Alignment via Cycle-teaching（通过循环教学的集合半监督实体对齐）

2. Authors: Weiqing Liu, Xiaojie Yuan, Xin Lv, Lei Liu, Wei Zhou

3. Affiliation: 未清刘 - 北京邮电大学；Xiaojie Yuan, Xin Lv, Lei Liu, Wei Zhou - 中国科学院自动化研究所

4. Keywords: Entity Alignment, Semi-supervised Learning, Ensemble Learning, Diversity-aware Alignment Selection, Conflict Resolution

5. Urls: Paper: http://arxiv.org/abs/2203.06308v1, Github: None

6. Summary:

   - (1): 本文研究实体对齐问题，即在不同的知识图谱中寻找相同的实体。现有的基于嵌入的方法已取得了显著进展，但是数据缺乏仍然是一个重要挑战，半监督方法也存在着在新提出的训练数据中存在不正确的实体对齐的问题。
   
   - (2): 现有的半监督方法面临着错误对齐的问题，同时由于不充足的训练数据无法有效地对不同知识图谱之间进行对齐求解，这使得现有的实体对齐方法的性能难以得到进一步提升和保持稳定。本文提出的循环教学框架可以有效地解决现有问题。该框架的关键想法是同时训练多个分类器，并让每个分类器迭代地教导其后继者新的实体对齐。同时，本文提出了一种多样性感知对齐选取方法，以选择可靠的实体对齐。本文还设计了一种冲突解决机制来解决从其老师继承新的对齐方案的新分类器与其自行提出的方案之间的对齐冲突。多个分类器的最佳训练次序也经过精心设计以最大化总体性能。该循环教学框架的过程可以打破分类器学习能力的限制和降噪新的训练数据，从而改善实体对齐性能。
   
   - (3): 本文提出了一种集合半监督实体对齐的循环教学框架。在该框架中，使用多个分类器并进行循环教学，以降低训练数据噪声，增强分类器学习能力，同时避免对齐偏好选择。
   
   - (4): 本文通过在基准数据集上的实验验证了所提出的循环教学框架的有效性，当训练数据不足且新实体对齐包含噪声时，该框架显著优于现有模型，并取得了更好的对齐性能。
7. Methods: 

- (1): 本文提出了一种循环教学框架（CycTEA）来解决实体对齐问题。该框架利用多个分类器同时学习，同时通过迭代教导后继者新的实体对齐，以解决现有半监督方法存在的错误对齐问题。同时，该框架提出了一种多样性感知对齐选取方法，以选择可靠的实体对齐，并设计了一种冲突解决机制来解决分类器之间的对齐冲突。多个分类器的最佳训练顺序也经过精心设计，以实现总体性能的最大化。

- (2): 本文循环教学框架的具体实现包括以下步骤：首先，初始化每个分类器的实体嵌入向量，并训练第一个分类器。接着，循环进行以下步骤直到收敛：每次选择一个分类器，将另外两个分类器的对齐结果合并作为其训练数据，再基于当前对齐结果训练该分类器并更新它的实体嵌入向量。然后，利用该分类器更新后继者的实体对齐结果，纳入下一轮训练。在该过程中，多样性感知对齐选取方法用于选择可靠的实体对齐，冲突解决机制用于解决分类器之间的对齐冲突，而最佳训练顺序的设计则用于最大化总体性能。

- (3): 本文还通过一系列实验验证了循环教学框架的有效性和优越性。实验结果表明，与现有方法相比，该框架能够显著提高实体对齐性能，特别是在训练数据不足且新实体对齐包含噪声时表现出更好的鲁棒性。同时，实验结果还验证了多样性感知对齐选取方法和对齐顺序的设计对于提高实体对齐性能的重要性。





8. Conclusion:

- (1): 本文提出了一种新颖实用的循环教学框架，能有效解决实体对齐问题中的训练数据不足和噪声扩散等问题，对于加强实体对齐方法的鲁棒性和性能提升等方面具有重要的意义。

- (2): 创新点方面，本文提出的循环教学框架采用了多个分类器同时学习和循环教导的思想，以及多样性感知对齐选取和冲突解决机制等技术手段，为实体对齐问题的解决带来了新思路；在性能方面，实验结果表明，本文提出的循环教学框架在基准数据集上比现有方法具有更好的实体对齐性能，尤其是在训练数据不足和存在噪声扩散的情况下更加鲁棒，具有很高的应用价值；在工作量方面，本文提出的循环教学框架虽然需要训练多个分类器，但可以通过精细设计分类器训练顺序等技巧来最大化整体性能，减少训练成本。




