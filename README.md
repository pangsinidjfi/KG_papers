# 知识图谱全栈开发所需论文
Knowledge Graph Papers
Contributed by Song Rui(宋瑞)、Zhao Ke(赵克)、Chen Hangting(陈杭婷)、Li Nan(李楠)、Xing Zhezhe(邢哲哲)

## [Content](#content)

<table>
<tr><td colspan="2"><a href="#实体识别">1. 实体识别</a></td></tr>
<tr>
    <td>&emsp;<a href="#基本模型">1.1 基本模型</a></td>
    <td>&emsp;<a href="#远程监督">1.2 远程监督</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#词汇增强">1.3 词汇增强</a></td>   
    <td>&ensp;<a href="#嵌套实体">1.4 嵌套实体</a></td> 
</tr>
<tr>
    <td>&ensp;<a href="#迁移学习">1.5 迁移学习</a></td>   
</tr>
<tr><td colspan="2"><a href="#关系抽取">2. 关系抽取</a></td></tr>
<tr>
    <td>&emsp;<a href="#有监督">2.1 有监督</a></td>
    <td>&emsp;<a href="#半监督">2.2 半监督</a></td>
</tr>
<tr><td colspan="2"><a href="#实体关系联合抽取">3. 实体关系联合抽取</a></td></tr>
<tr><td colspan="2"><a href="#知识融合">5. 知识融合</a></td></tr>
<tr>
    <td>&emsp;<a href="#实体对齐">5.1 实体对齐</a></td>
    <td>&emsp;<a href="#实体消歧">5.2 实体消歧</a></td>
</tr>
<tr><td colspan="2"><a href="#知识问答">6. 知识问答</a></td></tr>
<tr><td colspan="2"><a href="#推荐系统">7. 推荐系统</a></td></tr>
<tr><td colspan="2"><a href="#知识图谱表示学习">8. 知识图谱表示学习</a></td></tr>
</table>

## [实体识别](#content)
### [基本模型](#content)
1. **Bidirectional LSTM-CRF Models for Sequence Tagging, 2015** [paper](https://arxiv.org/pdf/1508.01991.pdf)
    *Huang, Zhiheng, Wei Xu, and Kai Yu.*(√)
    
2. **Fast and Accurate Entity Recognition with Iterated Dilated Convolutions, EMNLP2017** [paper](https://arxiv.org/pdf/1702.02098.pdf)
    *Strubell E, Verga P, Belanger D, et al.*

3. **A Multi-task Approach for Named Entity Recognition in Social Media Data，ACL2017** [paper](https://www.aclweb.org/anthology/W17-4419.pdf)
    *Gustavo Aguilar, Suraj Maharjan, A. Pastor L´opez-Monroy. University of Houston*
    
4. **Empower Sequence Labeling with Task-Aware Neural Language Model，AAAI2018** [paper](https://arxiv.org/pdf/1709.04109.pdf)
    *Liyuan Liuy, Jingbo Shang et al. University of Illinois at Urbana-Champaign, University of Southern California, Shanghai Jiao Tong University*(√)
    
5. **Neural Chinese Named Entity Recognition via CNN-LSTM-CRF and Joint Training with Word Segmentation，WWW2019** [paper](https://arxiv.org/pdf/1905.01964.pdf)
    *Fangzhao Wu, Junxin Liu, Chuhan Wu.  Microsoft Research Asia,Tsinghua University*(√)
    
6. **CAN-NER: Convolutional Attention Network for Chinese Named Entity Recognition, NAACL2019** [paper](https://arxiv.org/pdf/1904.02141.pdf)
    *Yuying Zhu, Guoxin Wang, Borje F. Karlsson. Nankai University, Microsoft Research Asia*(√)
    
7. **A Neural Multi-digraph Model for Chinese NER with Gazetteers，ACL2019** [paper](https://www.aclweb.org/anthology/P19-1141.pdf)
    *Ruixue Ding, Pengjun Xie et al. Alibaba Group, Beihang University, Singapore University of Technology and Design*(√)

8. **TriggerNER: Learning with Entity Triggers as Explanations for Named Entity Recognition, ACL2020** [paper](https://www.aclweb.org/anthology/2020.acl-main.752.pdf)
    *Bill Yuchen Lin, Dong-Ho Lee, Ming Shen, Ryan Moreno et al. University of Southern California; Amazon*(√)
    
9. **Handling Rare Entities for Neural Sequence Labeling, ACL2020** [paper](https://www.aclweb.org/anthology/2020.acl-main.574.pdf)(×)

10. **Multi-Domain Named Entity Recognition with Genre-Aware and Agnostic Inference, ACL2020** [paper](https://www.aclweb.org/anthology/2020.acl-main.750.pdf)(√)

### [远程监督](#content)
或者少量样本，或者低资源的实体识别。

1. **Distantly Supervised NER with Partial Annotation Learning and Reinforcement Learning, COLING2018** [paper](https://www.aclweb.org/anthology/C18-1183.pdf)
[code](https://github.com/mianzhang/DSNER)
    *Yaosheng Yang, Wenliang Chen, Zhenghua Li, Zhengqiu He, Min Zhang.  Soochow University, China*(√)

2. **Reinforcement-based denoising of distantly supervised NER with partial annotation，EMNLP2019** [paper](https://www.aclweb.org/anthology/D19-6125.pdf)
    *Farhad Nooralahzadeh, Jan Tore Lønning, Lilja Øvrelid.    University of Oslo, Norway*(√)

3. **Improving Low-Resource Named Entity Recognition using Joint Sentence and Token Labeling, ACL2020** [paper](https://www.aclweb.org/anthology/2020.acl-main.523/)

### [词汇增强](#content)
1. **Chinese NER Using Lattice LSTM，ACL2018** [paper](https://arxiv.org/pdf/1805.02023.pdf)
    *Yue Zhang, and Jie Yang. Singapore University of Technology and Design*(√)
    
2. **CNN-Based Chinese NER with Lexicon Rethinking，IJCAI2019** [paper](https://pdfs.semanticscholar.org/1698/d96c6fffee9ec969e07a58bab62cb4836614.pdf)
    *Tao Gui et al. Fudan University, Shanghai, China*(√)
    
3. **CGN: Leverage Lexical Knowledge for Chinese Named Entity Recognition via Collaborative Graph Network, EMNLP2019** [paper](https://www.aclweb.org/anthology/D19-1396.pdf)
    *Dianbo Sui, Yubo Chen, Kang Liu, Jun Zhao, Shengping Liu.  Chinese Academy of Sciences, University of Chinese Academy of Sciences*(√)
    
4. **A Lexicon-Based Graph Neural Network for Chinese NER，EMNLP2019** [paper](https://www.aclweb.org/anthology/D19-1096.pdf)
    *Tao Gui, Yicheng Zou, Qi Zhang et al. Fudan University*(√)
5. **FLAT: Chinese NER Using Flat-Lattice Transformer，ACL2020** [paper](https://arxiv.org/pdf/2004.11795.pdf)
    *Xiaonan Li, Hang Yan, Xipeng Qiu, Xuanjing Huang, Fudan University*(√)
    
### [嵌套实体](#content)
1. **Bipartite Flat-Graph Network for Nested Named Entity Recognition，ACL2020** [paper](https://www.aclweb.org/anthology/2020.acl-main.571.pdf)
    *Ying Luo, Hai Zhao. Shanghai Jiao Tong University*(√)
    
2. **Named Entity Recognition as Dependency Parsing, ACL2020** [paper](https://arxiv.org/pdf/2005.07150.pdf) [code](https://github.com/juntaoy/biaffine-ner)
    *Queen Mary University London,UK. Google Research,Netherlands*(√)
    
3. **Pyramid: A Layered Model for Nested Named Entity Recognition, ACL2020** [paper](https://www.aclweb.org/anthology/2020.acl-main.525.pdf)
    *Jue Wang, Lidan Shou, Ke Chen, Gang Chen. Zhejiang University*(√)
	
4. **Multi-Domain Named Entity Recognition with Genre-Aware and Agnostic Inference, ACL2020** [paper](https://www.aclweb.org/anthology/2020.acl-main.750.pdf)
	*Jing Wang, Mayank Kulkarni, Daniel Preotiuc-Pietro. Bloomberg*(√)
	
5. **Neural Architectures for Nested NER through Linearization, ACL2019** [paper](https://www.aclweb.org/anthology/P19-1527.pdf)
	*Jana Strakova, Milan Straka, Jan Hajic. Charles University*(√)
	
    
### [迁移学习](#content)

1. **Adversarial Transfer Learning for Chinese Named Entity Recognition with Self-Attention Mechanism, ACL2018** [paper](https://www.aclweb.org/anthology/D18-1017.pdf)

## [关系抽取](#content)
### [有监督](#content)
1. **End-to-End Neural Relation Extraction with Global Optimization, ACL2017** [paper](https://www.aclweb.org/anthology/D17-1182.pdf)

2. **Incorporating Relation Paths in Neural Relation Extraction,EMNLP2017** [paper](https://www.aclweb.org/anthology/D17-1186.pdf)

3. **A Walk-based Model on Entity Graphs for Relation Extraction,ACL2018** [paper](https://www.aclweb.org/anthology/P18-2014.pdf)
    *Fenia Christopoulou, Makoto Miwa, Sophia Ananiadou. The University of Manchester, United Kingdom; Toyota Technological Institute, Nagoya* 

### [半监督](#content)
包含bootstrapping和远程监督，后者在神经网络中常用。其基本假设是：对于一个已有的知识图谱中的一个三元组，假设外部文档库中任何包含这对实体的句子，在一定程度上都反映了这种关系。缺点是会引入大量噪声。因此会有一些操作可以减少噪声：多示例学习；强化学习；预训练。

1. **Snowball : Extracting relations from large Plain-text collections，2000**（这篇太久了可以不看）
    *Agichtein E, Gravano L*
    
2. **Deep Residual Learning for Weakly-Supervised Relation Extraction，ACL2017** [paper](https://www.aclweb.org/anthology/D17-1191.pdf)

3. **Learning with Noise: Enhance Distantly Supervised Relation Extraction with Dynamic Transition Matrix，ACL2018** [paper](https://www.aclweb.org/anthology/P17-1040.pdf)

3. **Neural Snowball for Few-Shot Relation Learning，AAAI2020** [paper](https://arxiv.org/pdf/1908.11007v1.pdf)
    *Tianyu Gao, Xu Han,Maosong Sun et al. Tsinghua University and Search Product Center, WeChat Search Application Department, Tencent*
    
4. **Distilling Knowledge fromWell-Informed Soft Labels for Neural Relation Extraction,AAAI2020** [paper](https://aaai.org/ojs/index.php/AAAI/article/view/6509/6365)
    *Zhenyu Zhang, Xiaobo Shu, Bowen Yu, Tingwen Liu et al. Chinese Academy of Sciences*

## [实体关系联合抽取](#content)

1. **Relabel the Noise: Joint Extraction of Entities and Relations via Cooperative Multiagents, ACL2020** [paper](https://arxiv.org/abs/2004.09930)

## [知识融合](#content)
### [实体对齐](#content)
**实体对齐（Entity Alignment）**：将具有相同真实世界身份的实体从不同知识图(KGs)中连接起来的任务。

1. **Relation-Aware Entity Alignment for Heterogeneous Knowledge Graphs，IJCAI2019** [paper](https://www.ijcai.org/Proceedings/2019/0733.pdf)
    *Yuting Wu et al. Peking University, China; Lancaster University, U. K.*

### [实体消歧](#content)
**实体消歧（Entity Disambiguation）**：实体消歧是实体连接中最主要的一步，将同一个实体的不同名字连接到一起。实体连接（或者实体消歧）的主要流程为：给定一个富含一系列实体的知识库与已经标注好mention的语料，实体链接任务的目标是将每一个mention匹配到知识库中它所对应的实体上面，如果知识库中没有某一mention对应的实体项，则认为该mention不可链接到当前知识库，标记为NIL。实体链接系统主要包含三个模块，分别为Candidate Entity Generation, Candidate Entity Ranking, Unlinkable Mention Prediction。[知乎](https://zhuanlan.zhihu.com/p/81073607)
1. **Deep Joint Entity Disambiguation with Local Neural Attention，EMNLP2017** [paper](https://www.aclweb.org/anthology/D17-1277.pdf)
    *Octavian-Eugen Ganea and Thomas Hofmann, ETH Zurich*

## [知识问答](#content)

## [推荐系统](#content)

## [知识图谱表示学习](#content)
