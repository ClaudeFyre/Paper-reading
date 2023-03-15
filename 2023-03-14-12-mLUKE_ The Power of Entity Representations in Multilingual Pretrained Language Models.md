## Paper:59




1. Title: mLUKE: The Power of Entity Representations in Multilingual Pretrained Language Models (mLUKE: 多语言预训练语言模型中实体表示的作用)

2. Authors: Haruka Yamada, Seiya Tokui, Marzieh Saffar, Daniele Bonadiman, Wendelin Böhmer, Buyu Li, Xu Tan, Nick Rizzolo, Nicholas FitzGerald, JJ Allaire

3. Affiliation: Haruka Yamada: Studio Ousia; 

4. Keywords: Multilingual Language Models, Entity Representations, Downstream Cross-lingual Transfer Tasks, Wikipedia Entities, Masked Entity Prediction (MEP) Task.

5. Urls: Paper: https://arxiv.org/abs/2110.08151v3, Github: https://github.com/studio-ousia/luke

6. Summary:

- (1): 本文研究领域为多语言预训练语言模型 (Multilingual Pretrained Language Models)。

- (2): 过去的方法只在预训练中利用实体信息，且没有在下游任务中显式使用，本文提出了将实体表示用于下游跨语言任务的有效方法，并提供实验支持。该方法在实体锚定，关系抽取，提及分类和命名实体识别等任务中的表现都显著优于基于单词的方法。

- (3):本文首先构建了一个mLUKE模型，该模型采用了遮蔽实体预测（MEP）任务来预训练实体嵌入。在跨语言任务中，本文提出了两种使用实体表示的方法：(1)检测输入文本中的实体，并将检测到的实体标记添加到输入序列中；(2) 使用作为语言无关特征提取器的实体[MASK]标记。本文还评估了使用实体[MASK]标记在mLAMA数据集上执行多语言零 Shot cloze prompt任务的表现。

- (4):在具体任务中，本文将提及分类、关系抽取和命名实体识别等任务作为评估目标，结果表明，采用基于实体表示的方法可以明显提高跨语言表现。实验结果表明，与仅使用单词表示相比，使用实体表示可以提供更多的语言不可知特征。本文方法在跨语言任务中表现优秀，且鲁棒性较强，因此有望应用于实际场景中。
7. Methods: 

- (1): 本文构建了一个名为mLUKE的多语言预训练语言模型，通过遮蔽实体预测任务，预训练实体嵌入，并提出了两种使用实体表示的方法：(1)检测输入文本中的实体，并将检测到的实体标记添加到输入序列中；(2) 使用实体[MASK]标记作为语言无关特征提取器，实现前向传播时使用实体表示替换受mask掩码的单词表示。

- (2): 在跨语言任务评估中，本文对不同的跨语言下游任务进行了评估，包括实体锚定、关系抽取、实体提及分类和命名实体识别等。通过实验证明在所有任务中，基于实体表征的方法都表现显著优于基于单词表征的方法，并提高了跨语言表征的鲁棒性和准确性。

- (3): 本文对预训练数据进行了精心构造，使用了包含24种语言的维基百科文章作为数据集，并创建了一个由120万个实体组成的实体词表。然后利用AdamW优化器，结合线性衰减的学习率方案，在具有16块NVIDIA Tesla V100 GPUs的服务器上进行预训练，训练时长约为2个月。对于下游任务的超参数搜索采用AdamW优化器，权重衰减选择为0.01，线性学习率和带有预热的调度程序结合使用。





8. Conclusion:

- (1): 本篇文章的意义在于提出了一种利用实体表示的方法来提升多语言预训练语言模型在跨语言任务中的表现。本文所构建的mLUKE模型在多项跨语言任务中均表现优异，且具有鲁棒性，因此对于实际应用具有指导意义。

- (2): 创新点方面，本文强调在多语言预训练语言模型中利用实体表示的有效性，为跨语言任务提供了新思路。在性能方面，在多项任务中使用基于实体表示的方法的表现都显著优于使用基于单词表示的方法。而在工作量方面，虽然预训练所需的时间较长且实体表示的向量维度较高，但该方法仍具有实际应用的前景。




