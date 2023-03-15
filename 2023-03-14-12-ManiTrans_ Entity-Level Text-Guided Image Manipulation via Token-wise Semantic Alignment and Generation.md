## Paper:80




1. Title: ManiTrans: Entity-Level Text-Guided Image Manipulation via Token-wise Semantic Alignment and Generation （《ManiTrans: 利用令牌级别的语义对齐和生成的实体级别文本引导图像操作》）

2. Authors: Jinzhe Wang, Wenbin Li, Jiaxing Huang, Yanwei Fu, Mingwu Yao, Hanwang Zhang

3. Affiliation: Department of Electronic Engineering, Tsinghua University,  Beijing, China （清华大学电子工程系，中国北京）

4. Keywords: Text-Guided Image Manipulation, Entity-Level, Semantic Alignment, Transformer, Image Synthesis

5. URLs: 
Paper: http://arxiv.org/abs/2204.04428v1
Project Homepage: https://jawang19.github.io/manitrans/
Code: None

6. Summary: 

- (1):该论文的研究背景是图像操作和生成，特别是在语义水平上为图像增添或修改实体的现实世界任务。

- (2):过去的方法主要针对在虚拟或简单场景中修改图像外观或编辑少量对象，不够实用。本文提出一种新方法，利用文本引导实现在真实世界尺度上的实体级别图像操作，该任务要求编辑与文本描述一致的实体、保留文本无关区域并将修改后的实体自然地融入图像中。常用的解决该任务的 TGIM 方法难以识别和编辑实体属性，而本文提出的 ManiTrans 框架通过基于 Transformer 的图像合成实现对离散图像令牌序列的学习，并通过语义对齐模块和 Contrastive Language-Image Pre-training (CLIP) 模块定位和修改与文本相关的图像令牌。

- (3):文章所提出的算法框架称为 ManiTrans，由两个部分组成，即 Transformer based image synthesizer (Trans)和 entity-level semantic manipulator (Mani)。其中，Trans 是一个利用 transformer 架构实现的图像生成模型，Mani 则是一个在实体级别上进行语义操作的模块。该框架具有令牌级的语义对齐和生成能力，通过细粒度的实体识别和修改，可以更好地区分与文本相关和与文本无关的区域。

- (4):本文所提出的 ManiTrans 在 CUB、Oxford、COCO 等真实数据集上进行了实验，能够准确地区分与文本相关和与文本无关的区域，从而能够实现更精细、更灵活地操作。相比基准方法，本文提出的方法不仅可以操作单个实体的纹理/颜色，还能够更好地操作多个实体的结构，支持更多样化的文本引导。
7. Methods:

- (1): 本文的方法是提出一种新的文本引导图像操作框架，即 ManiTrans，它由两个部分组成，即 Transformer based image synthesizer (Trans) 和 entity-level semantic manipulator (Mani)。

- (2): Trans 模块采用基于 Transformer 的图像合成技术，将输入的文本描述与图像中的语义区域进行对齐，生成准确的实体级别操作结果。

- (3): Mani 模块实现语义操作的细节控制，即具体的文本引导下的实体级别图像操作，通过细粒度的实体识别和修改，可以更好地区分与文本相关和与文本无关的区域，实现对文本引导下实体的颜色、纹理、形状等多方面的操作。

- (4): 除了 Mani 和 Trans 模块之外，ManiTrans 还采用了对比学习模块 CLIP，用于定位和修改与文本相关的图像令牌，提供更精细、更灵活的实体级别操作。在训练时，ManiTrans 还采用了语义对齐损失，帮助模型捕获输入文本和操作后的图片之间的视觉语义对齐。在推理阶段，ManiTrans 采用语义对齐模块，定位与文本相关的图像令牌进行操作。

- (5): 本文采用了三个真实数据集 CUB、Oxford、COCO 进行了实验。实验结果表明，ManiTrans 可以精准地区分文本相关和文本无关区域，实现更加精细、灵活的操作，相比基准方法具有更好的性能。





8. Conclusion: 
- (1): 本文的意义在于，首次研究了实体级别文本引导图像操作这一新领域，并提出了 ManiTrans 框架。该框架可以更加精细、灵活地操作图像，可用于许多工业应用和辅助视障人士等领域。

- (2): 创新点方面，本文提出了文本引导的实体级别图像操作框架 ManiTrans，引入了语义对齐和生成的技术，并应用 Transformer 架构实现图像生成。性能方面，实验结果表明，ManiTrans 可以精准地区分文本相关和文本无关区域，相比基准方法具有更好的性能。工作量方面，本文需要进行大量的实验和数据处理，但算法框架相对简单且易于理解。

Note: 
- (1) 中的 "ManiTrans"、"文本引导的实体级别图像操作"、"视障人士"、"Transformer" 均为 proper nouns，应标注为英文。
- (2) 中的三个维度，即创新点、性能、工作量，应分别给出评价。




