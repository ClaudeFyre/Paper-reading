## Paper:47




1. Title: Chemical Identification and Indexing in PubMed Articles via BERT and Text-to-Text Approaches (通过BERT和文本到文本方法在PubMed文章中进行化学物质鉴定和索引)
                 
                 2. Authors: Sufeng Leng, Jiahua Jin, Dequan Zheng, Dongfang Li, Zhiyong Lu, Dongcai Ye
                 
                 3. Affiliation: 麻省理工学院，哈佛医学院和医疗科技联合中心（MIT-IBM），哈佛大学
                 
                 4. Keywords: chemical identification, chemical indexing, named entity recognition, entity-linking, BERT, generative language model
                 
                 5. Urls: http://arxiv.org/abs/2111.15622v1 , Github: None

      
                 6. Summary: 

                    - (1): 本文的研究背景来自于一个基于生物创意七赛第二阶段挑战，即命名实体识别（Named Entity Recognition）、实体链接（Entity Linking）和主题索引任务。在此任务中，文本的实体和主题限制在化学物质上。 

                    - (2): 本文作者发现，命名实体识别是一个众所周知的问题。在本文实验中，使用基于BERT的BioMegatron模型得到了最佳的命名实体识别效果。对于实体链接，作者使用SAE （Self-Alignment Pretraining）预训练其BioBERT，并基于SAP（Self-Alignment Pretraining）之间的余弦相似度连接实体。虽然在命名实体识别实验中取得了成功，但是对于化学物质索引任务来说，依然存在挑战。为了改善问题，作者使用新颖的text-to-text方法，利用生成语言模型（如T5和GPT）进行命名实体识别和实体链接。该方法取得了鼓舞人心的结果。

                    - (3): 本文提出了一种文本到文本方法，用于化学物质鉴定和索引。该方法包括两种子任务：命名实体识别和实体链接。命名实体识别任务使用BioMegatron模型进行，实体链接使用SAE预训练BioBERT并基于SAP之间的余弦相似度连接实体。使用文本到文本方法基于生成语言模型（如T5和GPT）进行命名实体识别和实体链接。

                    - (4): 本文评估了不同方法在命名实体识别、实体链接和化学物质鉴定与索引上的性能，并对结果进行了比较。本文实验显示，BERT-based BioMegatron模型在命名实体识别方面具有最佳性能，T5和GPT等生成语言模型也能够近似于最佳方法，实现了更好的性能表现。在实体链接任务中，作者提出的SAE-pretrained BioBERT方法取得了最佳效果。 即使被鉴定化合物经历了变异，该方法仍然比传统方法更加鲁棒。
7. Methods:

- (1): 本文采用了命名实体识别（Named Entity Recognition，简称NER）、实体链接（Entity Linking，简称EL）和主题索引任务的文本到文本方法，用于化学物质鉴定和索引。其中，命名实体识别任务使用基于BioMegatron的BERT模型，并得到了最佳的命名实体识别效果。在此基础上，作者采用SAE预训练的BioBERT模型，基于余弦相似度连接实体，从而扩展了BERT模型应用于实体链接任务的能力。为了解决化学物质索引任务的挑战，作者采用了新颖的text-to-text方法，利用生成语言模型（如T5和GPT）进行命名实体识别和实体链接，取得了鼓舞人心的实验结果。
 
- (2): 实验评估中，本文比较了不同方法在命名实体识别、实体链接和化学物质鉴定与索引上的性能，并展示了相应的结果。本文实验显示，BERT-based BioMegatron模型在命名实体识别方面具有最佳性能，T5和GPT等生成语言模型也能够近似于最佳方法，实现了更好的性能表现。在实体链接任务中，作者提出的SAE-pretrained BioBERT方法取得了最佳效果。即使被鉴定化合物经历了变异，该方法仍然比传统方法更加鲁棒。

- (3): 本文用于实验的数据集是BioCreative VII Track 2提供的、由150篇full-text PubMed文章构成的数据集。每篇文章均具有标记的化学实体和化学物质主题。使用该数据集进行命名实体识别、实体链接和化学物质鉴定与索引任务的实验，并对实验结果进行了量化的评估。同时，作者为了实现text-to-text方法，在BioCreative VII Track 1的大规模子任务数据、BioCreative V挑战的CDR和CHEMDNER数据等进行了大规模的数据集构建实验。





8. Conclusion:

- (1): 本研究的意义在于，提出了一种新颖的基于文本到文本的方法，用于化学物质的鉴定和索引。同时，通过使用最先进的自然语言处理技术，如BERT和T5等生成语言模型，提高了命名实体识别和实体链接的精度，并在化学物质鉴定和索引任务中取得了很好的实验结果。

- (2): 创新点：本文提出了一种新颖的text-to-text方法，用于化学物质鉴定和索引，提高了命名实体识别和实体链接的精度。性能：在命名实体识别和实体链接方面，本文中提出的各种方法均与最佳方法相近，表现出了较好的性能。工作量：作者为实现text-to-text方法，在大规模数据集的构建方面付出了较大的工作量。




