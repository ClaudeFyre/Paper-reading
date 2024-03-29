## Paper:68




1. Title: EntityCS: Improving Zero-Shot Cross-lingual Transfer with Entity-Centric Code Switching (基于实体的混码技术提高零样本跨语言转移)
                 
                 2. Authors: Yanlin Luo, Xinyi Wang, Huishan Lang, Yingyan Zhou, Jie Zhou, Jianfeng Gao


                 3. Affiliation: 华为诺亚方舟实验室


                 4. Keywords: reinforcement learning, cross-lingual transfer, pre-trained language models, entity-centric code switching, natural language understanding


                 5. Urls: http://arxiv.org/abs/2210.12540v2, Github: https://github.com/huawei-noah/noah-research/tree/master/NLP/EntityCS

 
                 6. Summary:


                    - (1):该研究所关注的是跨语言的NLU任务，在零样本的情况下通过使用预训练语言模型来实现不同语言之间的转换。尽管现有的跨语言模型已经有了一定的进展，但在存在低资源语言的情况下，如何提高低资源语言的效果仍是一个瓶颈问题。
 
                    - (2):过去的方法主要是使用基于字典和平行句子的数据增强方法来实现跨语言转移。然而，这些方法可能会存在一些问题，例如字典法忽略了语义，打乱词语后句子的语法可能会变得无效。为了克服这些问题，本文提出了EntityCS方法，该方法利用基于实体的混码技术，以在不破坏语法的前提下捕捉跨语言语义信息。使用Wikidata和英文维基百科构建EntityCS语料库，并采用了面向实体的遮罩策略来改善实体识别。该方法提高了四个实体相关任务的性能，其中事实检索任务的性能增加了10％。
 
                    - (3):本研究提出的EntityCS方法使用基于实体的混码技术。在构建EntityCS语料库时，我们采用维基数据和英文维基百科来切换实体到其在其他语言中的对应项。然后，我们在此语料库上采用了面向实体的遮罩策略进行训练，以捕捉跨语言语义信息。
  
                    - (4):该方法在四个实体相关任务中都取得了不错的性能，表现出可行性和有效性。其中，在事实检索任务中取得了10％的性能提升，说明在跨语言NLU任务中使用基于实体的混码技术进行数据增强的有效性。
7. Methods: 

- (1): 本文的方法针对跨语言的NLU任务，在零样本的情况下如何提高不同语言之间的转换效果。本文提出了EntityCS方法，利用基于实体的混码技术来实现数据增强，以在不破坏语法的前提下捕捉跨语言语义信息。构建EntityCS语料库，使用Wikidata和英文维基百科来切换实体到其在其他语言中的对应项。使用面向实体的遮罩策略来改善实体识别。 

- (2): 研究使用不同的遮罩策略进行实验，其中包括基于实体的遮罩和基于非实体的遮罩，通过预测遮罩实体来预测跨语言语义信息，旨在将语言信息编码到预训练语言模型中。 对实体相关任务进行了测试，包括命名实体识别（NER）、事实检索、槽填充和词义消歧（WSD），评估零样本跨语言转移的能力。

- (3): 构建EntityCS语料库的具体步骤为：利用英文维基百科提取数据，记录wikilinks，采用SpaCy进行句子分割，以Wikidata作为实体数据库。以英语作为原始语种，获取实体对应的多语种ID，筛选出具有完整跨语言实体信息的语言作为目标语种，最终构建包含54.5万英语句子和104万实体的EntityCS语料库。

- (4): 本文使用四个实体相关任务，分别是命名实体识别（NER）、事实检索、槽填充和词义消歧（WSD）。对于实体识别任务，采用基于实体的遮罩策略，并取得了1-2％的性能提升。对于事实检索任务，采用不同的策略进行实验。实验结果表明，EntityCS方法对跨语言NLU任务的效果有所提高。





8. Conclusion: 

- (1): 本文提出了一种基于实体的混码技术来改进零样本跨语言转移的方法，着重解决了低资源语言的问题。研究表明，EntityCS方法在四个实体相关任务中取得了不错的性能，具有一定的可行性和有效性。 

- (2): 创新点：EntityCS方法采用基于实体的混码技术来实现数据增强，以在不破坏语法的前提下捕捉跨语言语义信息；性能方面，方法提高了四个实体相关任务的性能，其中事实检索任务性能增加了10%；工作量方面，构建EntityCS语料库的工作较为繁琐。




