## Paper:53




1. Title: RNN Transducers for Nested Named Entity Recognition with constraints on alignment for long sequences (基于约束对齐的长序列嵌套命名实体识别的RNN传导器)
 
                 2. Authors: Zhuosheng Zhang, Qi Zhang, Fen Lin, Weiran Xu, Buzhou Tang
 
                 3. Affiliation: Department of Computer Science and Technology, East China Normal University(华东师范大学计算机科学与技术系)
 
                 4. Keywords: Named Entity Recognition, RNN Transducer, constrained alignment, nested entities, overlapping entities
 
                 5. Urls: http://arxiv.org/abs/2203.03543v1 , Github: None
 
                 6. Summary:
 
                    - (1):本文研究的背景是命名实体识别（NER），旨在解决命名实体嵌套、命名实体重叠和命名实体位置识别等问题。
 
                    - (2):过去的方法包括条件随机场，序列到序列模型或利用问答框架。但是它们不适用于具有大本体的嵌套和重叠跨度以及预测实体的位置。为了填补这一空白，本文引入了一种新的NER模型-- RNN传导器(RNN-T)。这些模型使用成对的输入和输出序列进行训练，而无需明确指定它们之间的对齐，类似于其他序列到序列模型。RNN-T模型使用损失函数学习对齐，该函数对所有对齐求和。然而，在NER任务中，单词和目标标签之间的对齐是从人类注释中提取出来的。我们提出了一种固定对准的RNN-T模型，该模型利用给定的对准，同时保留了RNN-T模型的输出依赖性建模等优点。作为更一般的情况，我们还提出了一种约束对齐模型，用户可以指定给定输入对准的松弛程度，模型将在给定约束范围内学习对齐。换句话说，我们提出了一系列序列到序列模型，其中可以在可用时利用输入和目标序列之间的对齐。 通过在具有多个嵌套本体的具有挑战性的实际医学NER任务上进行实证实验，我们证明了我们的固定对准模型优于标准RNN-T模型，将F1-score从0.70提高到0.74。
 
                    - (3):本文提出了一种专门针对RNN传导器的NER任务的方法，引入了固定对准和约束对准的损失机制，优于常规的RNN传导器的效果。在NER任务上，限制对齐的RNN传导器（c-RNN-T）比常规的RNN传导器表现更好。此外，在医学NER任务上，固定对齐的RNN传导器（c-RNN-T-fixed）进一步提高了F1分数，并将其从0.70提高到0.74。
  
                    - (4):本文提出的方法在NER任务中表现良好，特别是固定对齐的RNN传导器在多嵌套本体的医学NER任务中表现优异，F1-score从0.70提高到0.74。因此，本文的方法可用于处理嵌套实体和重叠实体的NER任务。





8. Conclusion:
- (1): 本文的意义在于提出了一种新型的嵌套命名实体识别模型，可处理具有多个嵌套本体和重叠实体的NER任务。
 
- (2): 创新点：引入了RNN-T模型，并提出了固定对齐和约束对齐的损失机制。实验结果表明，c-RNN-T模型优于常规的RNN-T模型，固定对齐的模型进一步提高了F1分数；性能方面，在医学NER任务中表现良好，F1-score从0.70提高到0.74；工作量方面，本文方法需要的标注工作相对较少，只需提供词和目标标签之间的对齐即可。




