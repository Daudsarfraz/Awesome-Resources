# Transformers in Reinforcement Learning: A Survey

This repo contains a detailed list of research papers using Transformers in Reinforcement Learning. 

It is used for our survey paper [Transformers in Reinforcement Learning: A Survey](https://arxiv.org/pdf/2307.05979.pdf)

If you use it, please cite:

```
@article{agarwal2023transformers,
  title={Transformers in Reinforcement Learning: A Survey},
  author={Agarwal, Pranav and Rahman, Aamer Abdul and St-Charles, Pierre-Luc and Prince, Simon JD and Kahou, Samira Ebrahimi},
  journal={arXiv preprint arXiv:2307.05979},
  year={2023}
}
```

The list of papers are divided into multiple categories as elaborated below taking into account the use of Transformers in the field of Reinforcement Learning.

---

## Overview
- [Representation Learning](#representation-learning)
- [World Model](#world-model)
- [Reward Learning](#reward-learning)
- [Policy Learning](#policy-leaning)
- [Training Strategy](#training-strategy)
- [Explainability](#explainability)
- [Applications](#applications)
     * [Robotics](#robotics)
     * [Medical](#medical)
     * [Text Audio and Vision](#text-audio-vision)
     * [Edge and Cloud Computing](#edge-and-cloud-computing)
     * [Combinatorial Optimization](#combinatorial-optimzation)
     * [Environment](#environment)
     * [Scheduling](#scheduling)
     * [Trading](#trading)
     * [Hyperparameter Optimzation](#hyperparameter-optimzation)
---

## Representation Learning

* *My Body is a Cage: the Role of Morphology in Graph-Based Incompatible Control* [[Paper](https://arxiv.org/abs/2010.01856)] ***Apr 2021***

   Vitaly Kurin, Maximilian Igl, Tim Rocktäschel, Wendelin Boehmer, Shimon Whiteson
   
* *The Sensory Neuron as a Transformer: Permutation-Invariant NeuralNetworks for Reinforcement Learning* [[Paper](https://arxiv.org/abs/2109.02869)] ***Sept 2021***

   Yujin Tang, David Ha   
   
* *CoBERL: Contrastive BERT for Reinforcement Learning* [[Paper](https://arxiv.org/abs/2107.05431)] ***Feb 2022***

   Andrea Banino, Adrià Puidomenech Badia, Jacob Walker, Tim Scholtes, Jovana Mitrovic, Charles Blundell
   
* *Structure-Aware Transformer Policy for Inhomogeneous Multi-Task Reinforcement Learning* [[Paper](https://openreview.net/forum?id=fy_XRVHqly)] ***Mar 2022***

   Sunghoon Hong, Deunsol Yoon, Kee-Eung Kim   
   
* *Efficient Spatiotemporal Transformer for Robotic Reinforcement Learning* [[Paper](https://ieeexplore.ieee.org/document/9807399)] ***June 2022***

   Yiming Yang, Dengpeng Xing, Bo Xu  
   
* *Learning to Navigate in Interactive Environments with the Transformer-based Memory* [[Paper](https://embodied-ai.org/papers/2022/24.pdf)] ***June 2022***

   Weiyuan Li, Ruoxin Hong, Jiwei Shen, Yue Lu   
  
* *CtrlFormer: Learning Transferable State Representation for Visual Control via Transformer* [[Paper](https://arxiv.org/abs/2206.08883)] ***June 2022***

   Yao Mu, Shoufa Chen, Mingyu Ding, Jianyu Chen, Runjian Chen, Ping Luo
   
* *TVENet: Transformer-Based Visual Exploration Network for Mobile Robot in Unseen Environment* [[Paper](https://ieeexplore.ieee.org/document/9795177)] ***June 2022***

   Tianyao Zhang, Xiaoguang Hu, Jin Xiao, Guofeng Zhang    
   
* *StARformer: Transformer with State-Action-Reward Representations for Visual Reinforcement Learning* [[Paper](https://arxiv.org/pdf/2110.06206.pdf)] ***July 2022***

   Jinghuan Shang, Kumara Kahatapitiya, Xiang Li, Michael S. Ryoo

* *Multi-granularity scenarios understanding network for trajectory prediction* [[Paper](https://link.springer.com/article/10.1007/s40747-022-00834-2)] ***Aug 2022***

   Biao Yang, Jicheng Yang, Rongrong Ni, Changchun Yang,  Xiaofeng Liu 
   
* *One for All: One-stage Referring Expression Comprehension with Dynamic Reasoning* [[Paper](https://www.sciencedirect.com/science/article/pii/S0925231222012899)] ***Oct 2022***

   Zhipeng Zhang, Zhimin Wei, Zhongzhen Huang, Rui Niu, Peng Wang 
 
* *Unsupervised Learning of Temporal Abstractions with Slot-based Transformers* [[Paper](https://arxiv.org/abs/2203.13573)] ***Nov 2022***

   Anand Gopalakrishnan, Kazuki Irie, Jürgen Schmidhuber, Sjoerd van Steenkiste   
   
---

## World Model

* *Improving Sample Efficiency of Value Based Models Using Attention and Vision Transformers* [[Paper](https://arxiv.org/abs/2202.00710)] ***Feb 2022***

   Amir Ardalan Kalantari, Mohammad Amini, Sarath Chandar, Doina Precup
   
* *Dreaming with Transformers* [[Paper](http://aaai-rlg.mlanctot.info/papers/AAAI22-RLG_paper_24.pdf)] ***Feb 2022***

   Catherine Zeng, Jordan Docter, Alexander Amini, Igor Gilitschenski, Ramin Hasani and Daniela Rus 
   
* *TransDreamer: Reinforcement Learning with Transformer World Models* [[Paper](https://arxiv.org/abs/2202.09481)] ***Feb 2022***

   Chang Chen, Yi-Fu Wu, Jaesik Yoon, Sungjin Ahn
   
* *A model-based approach to meta-Reinforcement Learning: Transformers and tree search* [[Paper](https://arxiv.org/abs/2208.11535)] ***Aug 2022***

   Brieuc Pinon, Jean-Charles Delvenne, Raphaël Jungers    
   
* *Transformers are Sample Efficient World Models* [[Paper](https://arxiv.org/abs/2209.00588)] ***Sep 2022***

   Vincent Micheli, Eloi Alonso, François Fleuret
   
* *Masked World Models for Visual Control* [[Paper](https://arxiv.org/abs/2206.14244)] ***Nov 2022***

   Younggyo Seo, Danijar Hafner, Hao Liu, Fangchen Liu, Stephen James, Kimin Lee, Pieter Abbeel
   
* *Transformers-Based World Models Are Happy With 100k Interactions* [[Paper](https://openreview.net/pdf?id=TdBaDGCpjly)] ***Nov 2022***

   Jan Robine, Jan_Robine, Marc Höftmann, Tobias Uelwer, Stefan Harmeling


---

## Reward Learning
* *Comparing BERT-based Reward Functions for Deep Reinforcement Learning in Machine Translation* [[Paper](https://aclanthology.org/2022.wat-1.2.pdf)] ***Oct 2022***

   Yuki Nakatani, Tomoyuki Kajiwara, Takashi Ninomiya
 

---

## Policy Leaning

* *UPDeT: Universal Multi-agent Reinforcement Learning via Policy Decoupling with Transformers* [[Paper](https://arxiv.org/abs/2101.08001)] ***Feb 2021***

   Siyi Hu, Fengda Zhu, Xiaojun Chang, Xiaodan Liang 
   
* *Offline Reinforcement Learning as One Big Sequence Modeling Problem* [[Paper](https://arxiv.org/abs/2106.02039)] ***Jun 2021***

   Michael Janner, Qiyang Li, Sergey Levine
   
* *Decision Transformer: Reinforcement Learning via Sequence Modeling* [[Paper](https://arxiv.org/abs/2106.01345)] ***Jun 2021***

   Lili Chen, Kevin Lu, Aravind Rajeswaran, Kimin Lee, Aditya Grover, Michael Laskin, Pieter Abbeel, Aravind Srinivas, Igor Mordatch
   
* *A Novel Deep Reinforcement Learning Based Stock Direction Prediction using Knowledge Graph and Community Aware Sentiments* [[Paper](https://arxiv.org/abs/2107.00931)] ***July 2021***

   Anil Berk Altuner, Zeynep Hilal Kilimci   
   
* *Pretraining for Language Conditioned Imitation with Transformers* [[Paper](https://openreview.net/forum?id=eCPCn25gat)] ***Sept 2021***

   Aaron L Putterman, Kevin Lu, Igor Mordatch, Pieter Abbeel 
   
* *CubeTR: Learning to Solve the Rubik's Cube using Transformers* [[Paper](https://openreview.net/forum?id=wGLGG4918oc)] ***Sept 2021***

   Mustafa Ebrahim Chasmai    
  
* *Transfer learning with causal counterfactual reasoning in Decision Transformers* [[Paper](https://arxiv.org/abs/2110.14355)] ***Oct 2021***

   Ayman Boustati, Hana Chockler, Daniel C. McNamee    
   
* *Offline Pre-trained Multi-Agent Decision Transformer: One Big Sequence Model Tackles All SMAC Tasks* [[Paper](https://arxiv.org/abs/2112.02845)] ***Dec 2021***

   Linghui Meng, Muning Wen, Yaodong Yang, Chenyang Le, Xiyun Li, Weinan Zhang, Ying Wen, Haifeng Zhang, Jun Wang, Bo Xu 

 * *Switch Trajectory Transformer with Distributional Value Approximation for Multi-Task Reinforcement Learning* [[Paper](https://arxiv.org/abs/2203.07413)] ***Mar 2022***

   Qinjie Lin, Han Liu, Biswa Sengupta  
   
* *FedFormer: Contextual Federation with Attention in Reinforcement Learning* [[Paper](https://arxiv.org/abs/2205.13697)] ***May 2022***

   Liam Hebert, Lukasz Golab, Pascal Poupart, Robin Cohen   

* *Transformer with Memory Replay* [[Paper](https://arxiv.org/abs/2205.09869)] ***May 2022***

   Rui Liu, Barzan Mozafari
   
* *Online Decision Transformer* [[Paper](https://arxiv.org/abs/2202.05607)] ***July 2022***

   Qinqing Zheng, Amy Zhang, Aditya Grover   

* *Multi-Game Decision Transformers* [[Paper](https://arxiv.org/abs/2205.15241)] ***May 2022***

   Kuang-Huei Lee, Ofir Nachum, Mengjiao Yang, Lisa Lee, Daniel Freeman, Winnie Xu, Sergio Guadarrama, Ian Fischer, Eric Jang, Henryk Michalewski, Igor Mordatch
 
 * *Prompting Decision Transformer for Few-Shot Policy Generalization* [[Paper](https://mxu34.github.io/PromptDT/)] ***June 2022***

   Mengdi Xu, Yikang Shen, Shun Zhang, Yuchen Lu, Ding Zhao, Joshua B. Tenenbaum, Chuang Gan
   
* *Offline Pre-trained Multi-Agent Decision Transformer: One Big Sequence Model Tackles All SMAC Tasks* [[Paper](https://arxiv.org/abs/2112.02845)] ***Jun 2022***

   Linghui Meng, Muning Wen, Yaodong Yang, Chenyang Le, Xiyun Li, Weinan Zhang, Ying Wen, Haifeng Zhang, Jun Wang, Bo Xu  
   
* *Transformers are Meta-Reinforcement Learners* [[Paper](https://arxiv.org/abs/2206.06614)] ***June 2022***

   Luckeciano C. Melo   

* *Transformer-based Value Function Decomposition for Cooperative Multi-agent Reinforcement Learning in StarCraft* [[Paper](https://arxiv.org/abs/2208.07298)] ***Aug 2022***

   Muhammad Junaid Khan, Syed Hammad Ahmed, Gita Sukthankar 
   
* *Transformer-Based Deep Reinforcement Learning in VizDoom* [[Paper](https://link.springer.com/content/pdf/10.1007/978-3-031-15168-2_9.pdf)] ***Aug 2022***

   Vitalii Sopov, Ilya Makarov
   
* *Q-learning Decision Transformer: Leveraging Dynamic Programming for Conditional Sequence Modelling in Offline RL* [[Paper](https://arxiv.org/abs/2209.03993)] ***Oct 2022***

   Taku Yamagata, Ahmed Khalil, Raul Santos-Rodriguez   
   
* *Bootstrapped Transformer for Offline Reinforcement Learning* [[Paper](https://arxiv.org/abs/2206.08569)] ***Oct 2022***

   Kerong Wang, Hanye Zhao, Xufang Luo, Kan Ren, Weinan Zhang, Dongsheng Li  
   
* *Relational Reasoning via Set Transformers: Provable Efficiency and Applications to MARL* [[Paper](https://arxiv.org/abs/2209.09845)] ***Oct 2022***

   Fengzhuo Zhang, Boyi Liu, Kaixin Wang, Vincent Y. F. Tan, Zhuoran Yang, Zhaoran Wang

* *Multi-Agent Reinforcement Learning is a Sequence Modeling Problem* [[Paper](https://arxiv.org/abs/2205.14953)] ***Oct 2022***

   Muning Wen, Jakub Grudzien Kuba, Runji Lin, Weinan Zhang, Ying Wen, Jun Wang, Yaodong Yang
   
* *You Can't Count on Luck: Why Decision Transformers and RvS Fail in Stochastic Environments* [[Paper](https://arxiv.org/abs/2205.15967)] ***Nov 2022***

   Keiran Paster, Sheila McIlraith, Jimmy Ba
   
* *Deep Transformer Q-Networks for Partially Observable Reinforcement Learning* [[Paper](https://arxiv.org/abs/2206.01078)] ***Nov 2022***

   Kevin Esslinger, Robert Platt, Christopher Amato 

---

## Training Strategy
* *Stabilizing Transformers for Reinforcement Learning* [[Paper](https://arxiv.org/abs/1910.06764)] ***Oct 2019***

   Emilio Parisotto, H. Francis Song, Jack W. Rae, Razvan Pascanu, Caglar Gulcehre, Siddhant M. Jayakumar, Max Jaderberg, Raphael Lopez Kaufman, Aidan Clark, Seb Noury, Matthew M. Botvinick, Nicolas Heess, Raia Hadsell
   
* *Semi-supervised Offline Reinforcement Learning with Pre-trained Decision Transformers* [[Paper](https://openreview.net/forum?id=fwJWhOxuzV9)] ***Sept 2021***

   Catherine Cang, Kourosh Hakhamaneshi, Ryan Rudes, Igor Mordatch, Aravind Rajeswaran, Pieter Abbeel, Michael Laskin
   
* *Can Wikipedia Help Offline Reinforcement Learning?* [[Paper](https://arxiv.org/abs/2201.12122)] ***Jan 2022***

   Machel Reid, Yutaro Yamada, Shixiang Shane Gu
   
* *Evaluating Vision Transformer Methods for Deep Reinforcement Learning from Pixels* [[Paper](https://arxiv.org/abs/2204.04905)] ***Apr 2022***

   Tianxin Tao, Daniele Reda, Michiel van de Panne

---

## Explainability
* *ATTEXPLAINER: Explain Transformer via Attention by Reinforcement Learning* [[Paper](https://www.ijcai.org/proceedings/2022/0102.pdf)] ***July 2022***

   Runliang Niu, Zhepei Wei, Yan Wang, Qi Wang 

---

## Applications
### Robotics

* *Vision Transformer for Learning Driving Policies in Complex Multi-Agent Environments* [[Paper](https://arxiv.org/abs/2109.06514)] ***Sept 2021***

   Eshagh Kargar, Ville Kyrki
   
* *Neurosymbolic Learning for Robust and Reliable Intelligent Systems* [[Paper](https://dspace.mit.edu/bitstream/handle/1721.1/143249/Inala-jinala-PhD-EECS-2022-thesis.pdf?sequence=1&isAllowed=y)] ***Feb 2022***

   Jeevana Priya Inala  
   
* *Object Memory Transformer for Object Goal Navigation* [[Paper](https://arxiv.org/abs/2203.14708)] ***Mar 2022***

   Rui Fukushima, Kei Ota, Asako Kanezaki, Yoko Sasaki, Yusuke Yoshiyasu
   
* *End-to-End Trajectory Distribution Prediction Based on Occupancy Grid Maps* [[Paper](https://arxiv.org/abs/2203.16910)] ***Mar 2022***

   Ke Guo, Wenxi Liu, Jia Pan   
   
* *Learning Efficient Multi-agent Cooperative Visual Exploration* [[Paper](https://link.springer.com/chapter/10.1007/978-3-031-19842-7_29)] ***Oct 2022***

   Chao Yu, Xinyi Yang, Jiaxuan Gao, Huazhong Yang, Yu Wang, Yi Wu   
   
* *Augmenting Reinforcement Learning with Transformer-based Scene Representation Learning for Decision-making of Autonomous Driving* [[Paper](https://arxiv.org/abs/2208.12263)]***Aug 2022***

   Haochen Liu, Zhiyu Huang, Xiaoyu Mo, Chen Lv
   
* *TransNav: spatial sequential transformer network for visual navigation* [[Paper](https://academic.oup.com/jcde/article/9/5/1866/6679563)] ***Aug 2022***

   Kang Zhou, Huyin Zhang, Fei Li
   
---
### Medical


* *Reinforced Transformer for Medical Image Captioning* [[Paper](https://link.springer.com/chapter/10.1007/978-3-030-32692-0_77)] ***Oct 2019***

    Yuxuan Xiong, Bo Du, Pingkun Yan 

* *Improving Factual Completeness and Consistency of Image-to-Text Radiology Report Generation* [[Paper](https://aclanthology.org/2021.naacl-main.416/)] ***June 2021***

    Yasuhide Miura, Yuhao Zhang, Emily Tsai, Curtis Langlotz, Dan Jurafsky 

 * *Multi-constraint molecular generation based on conditional transformer, knowledge distillation and reinforcement learning* [[Paper](https://www.nature.com/articles/s42256-021-00403-1)] ***Oct 2021***

    Jike Wang, Chang-Yu Hsieh, Mingyang Wang, Xiaorui Wang, Zhenxing Wu, Dejun Jiang, Benben Liao, Xujun Zhang, Bo Yang, Qiaojun He, Dongsheng Cao, Xi Chen, Tingjun Hou   
    
* *Deep Reinforcement Learning and Docking Simulations for autonomous molecule generation in de novo Drug Design* [[Paper](https://dl.acm.org/doi/10.1145/3469877.3497694)] ***Dec 2021***

   Qian Wang, Hao Liu, Xiaotong Hu
  
* *Transformer-Based Generative Model Accelerating the Development of Novel BRAF Inhibitors* [[Paper](https://pubs.acs.org/doi/10.1021/acsomega.1c05145)] ***Dec 2021***

   Lijuan Yang, Guanghui Yang, Zhitong Bing, Yuan Tian, Yuzhen Niu, Liang Huang, Lei Yang
   
* *DrugEx v3: Scaffold-Constrained Drug Design with Graph Transformer-based Reinforcement Learning* [[Paper](https://chemrxiv.org/engage/chemrxiv/article-details/61aa8b58bc299c0b30887f80)] ***Dec 2021***

    Xuhan Liu, Kai Ye, Herman W. T. van Vlijmen, Adriaan P. IJzerman, Gerard J. P. van Westen 

* *Active Phase-Encode Selection for Slice-Specific Fast MR Scanning Using a Transformer-Based Deep Reinforcement Learning Framework* [[Paper](https://arxiv.org/abs/2203.05756)] ***Mar 2022***

    Yiming Liu, Yanwei Pang, Ruiqi Jin, Zhenchang Wang    
    
* *SIG-Former: monocular surgical instruction generation with transformers* [[Paper](https://link.springer.com/article/10.1007/s11548-022-02718-9)] ***July 2022***

    Jinglu Zhang, Yinyu Nie, Jian Chang, Jian Jun Zhang
    
* *Transformer-based Objective-reinforced Generative Adversarial Network to Generate Desired Molecules* [[Paper](https://www.ijcai.org/proceedings/2022/539)] ***July 2022***

    Chen Li, Chikashige Yamanaka, Kazuma Kaitoh, Yoshihiro Yamanishi   

* *RL Based Unsupervised Video Summarization Framework for Ultrasound Imaging* [[Paper](https://link.springer.com/chapter/10.1007/978-3-031-16902-1_3)] ***Sept 2022***

   Roshan P. Mathews, Mahesh Raveendranatha Panicker, Abhilash R. Hareendranathan, Yale Tung Chen, Jacob L. Jaremko, Brian Buchanan, Kiran Vishnu Narayan, Kesavadas Chandrasekharan , Greeta Mathews
    
* *DxFormer: A Decoupled Automatic Diagnostic System Based on Decoder-Encoder Transformer with Dense Symptom Representations* [[Paper](https://arxiv.org/pdf/2205.03755.pdf)] ***Dec 2022***

    Wei Chen, Cheng Zhong, Jiajie Peng, Zhongyu Wei
    
---
### Text Audio and Vision
* *Towards Reinforcement Learning for Pivot-based Neural Machine Translation with Non-autoregressive Transformer* [[Paper](https://arxiv.org/abs/2109.13097)] ***Sept 2021***

   Evgeniia Tokarchuk, Jan Rosendahl, Weiyue Wang, Pavel Petrushkov, Tomer Lancewicki, Shahram Khadivi, Hermann Ney
   
* *Corrective Guidance and Learning for Dialogue Management* [[Paper](https://dl.acm.org/doi/abs/10.1145/3459637.3482333)] ***Oct 2021***

   Mahdin Rohmatillah, Jen-Tzung Chien    
   
* *Goal-Directed Story Generation: Augmenting Generative Language Models with Reinforcement Learning* [[Paper](https://arxiv.org/abs/2112.08593)] ***Dec 2021***

   Amal Alabdulkarim, Winston Li, Lara J. Martin, Mark O. Riedl 
   
* *Adversarial Conversational Shaping for Intelligent Agents* [[Paper](https://neurips2021-nlp.github.io/papers/13/CameraReady/ENLSP_final_submission.pdf)] ***Dec 2021***

   Piotr Tarasiewicz, Sultan Kenjeyev, Ilana Sebag, Shehab Alshehabi 
   
* *FCSF-TABS: two-stage abstractive summarization with fact-aware reinforced content selection and fusion* [[Paper](https://link.springer.com/article/10.1007/s00521-021-06880-0)] ***Jan 2022***

   Mengli Zhang, Gang Zhou, Wanting Yu, Wenfen Liu, Ningbo Huang,  Ze Yu    
   
* *Audio Embeddings Help to Learn Better Dialogue Policies* [[Paper](https://ieeexplore.ieee.org/document/9688296)] ***Feb 2022***

   Asier López Zorrilla, M. Inés Torres, Heriberto Cuayáhuitl  

* *Reward Modeling for Mitigating Toxicity in Transformer-based Language Models* [[Paper](https://arxiv.org/abs/2202.09662)] ***Feb 2022***

   Farshid Faal, Ketra Schmitt, Jia Yuan Yu
   
* *Active Audio-Visual Separation of Dynamic Sound Sources* [[Paper](https://arxiv.org/abs/2202.00850)] ***Feb 2022***

   Sagnik Majumder, Kristen Grauman   
   
* *Bailando: 3D Dance Generation by Actor-Critic GPT with Choreographic Memory* [[Paper](https://arxiv.org/abs/2203.13055)] ***Mar 2022***
    
   Li Siyao, Weijiang Yu, Tianpei Gu, Chunze Lin, Quan Wang, Chen Qian, Chen Change Loy, Ziwei Liu    
   
* *Multi-Modal Instruction based Reinforcement Learning using MoME Transformer* [[Paper](https://www.techrxiv.org/articles/preprint/Multi-Modal_Instruction_based_Reinforcement_Learning_using_MoME_Transformer/19566040)] ***Apr 2022***

   Avish Kadakia, Sabah Mohammed  
   
* *Meta Policy Learning for Cold-Start Conversational Recommendation* [[Paper](https://arxiv.org/abs/2205.11788)] ***May 2022***

   Zhendong Chu, Hongning Wang, Yun Xiao, Bo Long, Lingfei Wu 
   
* *SILVER-BULLET-3D AT MANISKILL 2021: LEARNING-FROM-DEMONSTRATIONS AND HEURISTIC RULE-BASED METHODS FOR OBJECT MANIPULATION* [[Paper](https://openreview.net/pdf?id=rNhxaETVybc)] ***Jun 2022***

   Yingwei Pan, Yehao Li, Yiheng Zhang, Qi Cai, Fuchen Long, Zhaofan Qiu, Ting Yao, Tao Mei
      
* *TF-SOD: a novel transformer framework for salient object detection* [[Paper](https://link.springer.com/article/10.1007/s00521-022-07069-9)] ***July 2022***
    
   Yunzhou Zhang, Zhenyu Wang,  Yan Liu, Zhuo Wang, Sonya Coleman, Dermot Kerr    
   
* *Improving Multi-Document Summarization through Referenced Flexible Extraction with Credit-Awareness* [[Paper](https://aclanthology.org/2022.naacl-main.120/)] ***July 2022***

   Yun-Zhu Song, Yi-Syuan Chen, Hong-Han Shuai   
   
* *Emotion Aware Reinforcement Network for Visual Storytelling* [[Paper](https://link.springer.com/chapter/10.1007/978-3-031-15931-2_3)] ***Sept 2022***

   Xin Li, Hanqing Cai, Tianling Jiang, Chunping Liu,  Yi Ji

* *SURF: Semantic-level Unsupervised Reward Function for Machine Translation* [[Paper](https://aclanthology.org/2022.naacl-main.334/)] ***July 2022***

   Atijit Anuchitanukul, Julia Ive 
   
* *GenTUS: Simulating User Behaviour and Language in Task-oriented Dialogues with Generative Transformers* [[Paper](https://arxiv.org/abs/2208.10817)] ***Sept 2022***

   Hsien-chin Lin, Christian Geishauser, Shutong Feng, Nurul Lubis, Carel van Niekerk, Michael Heck, Milica Gasic 
      
* *Dynamic Dialogue Policy for Continual Reinforcement Learning* [[Paper](https://arxiv.org/abs/2204.05928)] ***Oct 2022***

   Christian Geishauser, Carel van Niekerk, Hsien-chin Lin, Nurul Lubis, Michael Heck, Shutong Feng, Milica Gašić  
   
* *Selective Token Generation for Few-shot Natural Language Generation* [[Paper](https://aclanthology.org/2022.coling-1.510.pdf)] ***Oct 2022***

   Daejin Jo, Taehwan Kwon, Eun-Sol Kim, Sungwoong Kim
   
* *Efficient Unsupervised Sentence Compression by Fine-tuning Transformers with Reinforcement Learning* [[Paper](https://arxiv.org/abs/2205.08221)] ***Nov 2022***

   Demian Ghalandari, Chris Hokamp, Georgiana Ifrim 
     
* *RLAS-BIABC: A Reinforcement Learning-Based Answer Selection Using the BERT Model Boosted by an Improved ABC Algorithm* [[Paper](https://dl.acm.org/doi/abs/10.1155/2022/7839840)] ***Jan 2023***

   Hamid Gharagozlou, Javad Mohammadzadeh, Azam Bastanfard, Saeed Shiry Ghidary
   
---
### Edge and Cloud Computing
* *Exploring reward efficacy in traffic management using deep reinforcement learning in intelligent transportation system* [[Paper](https://onlinelibrary.wiley.com/doi/full/10.4218/etrij.2021-0404)] ***April 2022***

   Ananya Paul, Sulata Mitra 
* *A Distributed Vehicle-assisted Computation Offloading Scheme based on DRL in Vehicular Networks* [[Paper](https://ieeexplore.ieee.org/document/9826050)] ***July 2022***

   Jiayue Wang, Hongbo Zhao, Haoqiang Liu, Liwei Geng, Zebin Sun 
* *Reinforced Transformer Learning for VSI-DDoS Detection in Edge Clouds* [[Paper](https://ieeexplore.ieee.org/document/9878326)] ***Sept 2022***

   Adil Bin Bhutto, Xuan Son Vu, Erik Elmroth, Wee Peng Tay, Monowar Bhuyan 
* *Actor-Critic with Transformer for Cloud Computing Resource Three Stage Job Scheduling* [[Paper](https://ieeexplore.ieee.org/document/9778883)] ***Sept 2022***

   Yanbo Xu, Jiakun Zhao 

---
### Combinatorial Optimzation
* *Attention-Based Learning for Combinatorial Optimization* [[Paper](https://dspace.mit.edu/bitstream/handle/1721.1/144893/Smith-smithcj-meng-eecs-2022-thesis.pdf?sequence=1&isAllowed=y)] ***May 2022***

   Carson Smith 

* *A Deep Reinforcement Learning Algorithm Using A New Graph Transformer Model for Routing Problems* [[Paper](https://link.springer.com/chapter/10.1007/978-3-031-16075-2_26)] ***Sept 2022***

   Yang Wang, Zhibin Chen
---

### Environment
* *Deep reinforcement learning for optimal well control in subsurface systems with uncertain geology* [[Paper](https://arxiv.org/abs/2203.13375)] ***Mar 2022***

   Yusuf Nasir, Louis J. Durlofsky  
   
* *Confidence Estimation Transformer for Long-term Renewable Energy Forecasting in Reinforcement Learning-based Power Grid Dispatching* [[Paper](https://arxiv.org/abs/2204.04612)] ***Apr 2022***

   Xinhang Li, Zihao Li, Nan Yang, Zheng Yuan, Qinwen Wang, Yiying Yang, Yupeng Huang, Xuri Song, Lei Li, Lin Zhang
   
* *A Hybrid Data-Driven Method for Low-Carbon Economic Energy Management Strategy in Electricity-Gas Coupled Energy Systems Based on Transformer Network and Deep Reinforcement Learning* [[Paper](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4089060)] ***Apr 2022***

   Bin Zhang, Weihao Hu, Xiao Xu, Zhenyuan Zhang, Zhe Chen
   
* *Stabilizing Voltage in Power Distribution Networks via Multi-Agent Reinforcement Learning with Transformer* [[Paper](https://arxiv.org/abs/2206.03721)] ***Jun 2022***

   Minrui Wang, Mingxiao Feng, Wengang Zhou, Houqiang Li
    
   
* *Toward Smart Multizone HVAC Control by Combining Context-Aware System and Deep Reinforcement Learning* [[Paper](https://ieeexplore.ieee.org/document/9776508)] ***May 2022***

   Xiangtian Deng, Yi Zhang, Yi Zhang, He Qi
---
### Scheduling

* *A Deep Reinforcement Learning Framework Based on an Attention Mechanism and Disjunctive Graph Embedding for the Job-Shop Scheduling Problem* [[Paper](https://ieeexplore.ieee.org/document/9757835)] ***Apr 2022***

   Ruiqi Chen, Wenxin Li, Hongbing Yang

* *An End-to-End Deep Reinforcement Learning Approach for Job Shop Scheduling* [[Paper](https://ieeexplore.ieee.org/document/9776116)] ***May 2022***

   Linlin Zhao, Weiming Shen, Chunjiang Zhang, Kunkun Peng 

* *Transformer-Based Reinforcement Learning for Pickup and Delivery Problems With Late Penalties* [[Paper](https://ieeexplore.ieee.org/document/9847118)] ***Aug 2022***

   Ke Zhang, Xi Lin, Meng Li 
   
* *Attention-based model and deep reinforcement learning for distribution of event processing tasks* [[Paper](https://www.sciencedirect.com/science/article/pii/S2542660522000580)] ***Aug 2022***

   Andriy Mazayev, Faroq Al-Tam, Noélia Correia 
       
---
### Trading
* *Relation-Aware Transformer for Portfolio Policy Learning* [[Paper](https://dl.acm.org/doi/abs/10.5555/3491440.3492081)] ***July 2020***
   
   Ke Xu1, Yifan Zhang1, Deheng Ye, Peilin Zhao, Mingkui Tan

* *A Novel Deep Reinforcement Learning Framework for Stock Portfolio Optimization* [[Paper](https://link.springer.com/chapter/10.1007/978-3-030-92307-5_24)] ***Dec 2021***

    Shaobo Hu, Hongying Zheng, and Jianyong Chen
---

### Hyperparameter Optimzation
* *AME: Attention and Memory Enhancement in Hyper-Parameter Optimization* [[Paper](https://openaccess.thecvf.com/content/CVPR2022/papers/Xu_AME_Attention_and_Memory_Enhancement_in_Hyper-Parameter_Optimization_CVPR_2022_paper.pdf)] ***June 2022***

    Nuo Xua, Jianlong Chang, Xing Nie, Chunlei Huo, Shiming Xiang and Chunhong Pan

---

































 




























 

 






  
