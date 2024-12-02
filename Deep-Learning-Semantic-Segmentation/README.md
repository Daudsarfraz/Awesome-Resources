# Deep-Learning-Semantic-Segmentation
A paper list of semantic segmentation using deep learning.

|network|VOC12|VOC12 with COCO|Pascal Context|CamVid|Cityscapes|ADE20K|Published In |
|:-----:|:--------:|:------------------:|:-----------------:|:---------:|:-------------:|:---------:|:-----------:|
|FCN-8s |62.2      |                    |37.8               |           |65.3           |           |CVPR 2015    |
|DeepLab|71.6      |                    |                   |           |               |           |ICLR 2015    |
|CRF-RNN|72.0      |74.7                |39.3               |           |               |           |ICCV 2015    |
|DeconvNet|72.5    |                    |                   |           |               |           |ICCV 2015    |
|DPN    |74.1      |77.5                |                   |           |               |           |ICCV 2015    |
|SegNet |          |                    |                   |50.2       |
|Dilation8|        |75.3                |                   |           |               |           |
|Deeplab v2|       |79.7                |45.7               |           |70.4           |           |PAMI         |
|FRRN B |          |                    |                   |           |71.8           |           |CVPR 2017    |
|G-FRNet|79.3      |                    |                   |68.0       |               |           |CVPR 2017    |
|GCN|              |82.2                |                   |           |76.9           |           |CVPR 2017    |
|SegModel|         |82.5                |                   |           |79.2           |           |CVPR 2017    |
|RefineNet|        |83.4                |47.3               |           |73.6           |40.7       |CVPR 2017    |
|PSPNet|82.6       |85.4                |                   |           |80.2           |           |CVPR 2017    |
|DIS|              |86.8                |                   |           |               |           |ICCV 2017    |
|SAC-multiple|     |                    |                   |           |78.1           |44.3       |ICCV 2017    |
|DeepLabv3|        |85.7                |                   |           |81.3           |           |arxiv 1706.05587|
|DUC-HDC|          |                    |                   |           |80.1           |           |WACV2018|
|DDSC|81.2         |                    |47.8               |70.9       |               |           |CVPR 2018|
|EncNet|82.9       |85.9                |51.7               |           |               |44.65      |CVPR 2018|
|DFN|82.7          |86.2                |                   |           |80.3           |           |CVPR 2018|
|DenseASPP|        |                    |                   |           |80.6           |           |CVPR 2018|
|UperNet|          |                    |                   |           |               |42.66      |ECCV 2018|
|PSANet|           |85.7                |                   |           |80.1           |43.77      |ECCV 2018|
|DeepLabv3+|       |87.8                |                   |           |82.1           |           |ECCV 2018|
|ExFuse|           |87.9                |                   |           |               |           |ECCV 2018|
|OCNet|            |                    |                   |           |81.2(81.7)     |45.08(45.45)|arxiv 1809.00916|
|DAN|              |                    |52.6               |           |78.2           |           |CVPR 2019|
|DPC|              |87.9                |                   |           |82.7           |           |NIPS 2018|
|CCNet|            |                    |                   |           |81.4           |45.22      |arxiv 1811.11721|
|GloRe|            |                    |                   |           |80.9           |           |CVPR 2019|
|TKCN|             |83.2                |                   |           |79.5           |           |ICME 2019|
|GCU|              |                    |                   |           |               |44.81      |NIPS 2018|
|DUpsampling|85.3  |88.1                |52.5               |           |               |           |CVPR 2019|
|FastFCN|          |                    |53.1               |           |               |44.34      |arxiv 1903.11816|
|GFF|              |                    |                   |           |82.3           |45.33      |arxiv 1904.01803|
|HRNetV2|          |                    |54.0               |           |81.6           |           |arxiv 1904.04514|

Semantic Segmentation论文整理
<!--more-->
# dataset


# 2D Semantic Segmentation
## 2014
- [**FCN**] Fully Convolutional Networks for Semantic Segmentation [[Paper1]](http://arxiv.org/abs/1411.4038) [[Paper2]](http://arxiv.org/abs/1605.06211) [[Slides1]](https://docs.google.com/presentation/d/1VeWFMpZ8XN7OC3URZP4WdXvOGYckoFWGVN7hApoXVnc) [[Slides2]](http://tutorial.caffe.berkeleyvision.org/caffe-cvpr15-pixels.pdf)
- [**DeepLab v1**] Semantic Image Segmentation With Deep Convolutional Nets and Fully Connected CRFs[[Code-Caffe]](https://bitbucket.org/deeplab/deeplab-public/) [[Paper]](http://arxiv.org/abs/1412.7062)

## 2015
- [**CRF as RNN**] Conditional Random Fields as Recurrent Neural Networks [[Project]](http://www.robots.ox.ac.uk/~szheng/CRFasRNN.html) [[Demo]](http://www.robots.ox.ac.uk/~szheng/crfasrnndemo) [[Paper]](http://arxiv.org/abs/1502.03240)
- [**DeconvNet**] Learning Deconvolution Network for Semantic Segmentation [[Project]](http://cvlab.postech.ac.kr/research/deconvnet/) [[Paper]](http://arxiv.org/abs/1505.04366) [[Slides]](http://web.cs.hacettepe.edu.tr/~aykut/classes/spring2016/bil722/slides/w06-deconvnet.pdf)
- [**U-Net**] U-Net: Convolutional Networks for Biomedical Image Segmentation [[Project]](http://lmb.informatik.uni-freiburg.de/people/ronneber/u-net/) [[Paper]](http://arxiv.org/abs/1505.04597)
- [**SegNet**] SegNet: A Deep Convolutional Encoder-Decoder Architecture for Image Segmentation [[Project]](http://mi.eng.cam.ac.uk/projects/segnet/) [[Paper]](http://arxiv.org/abs/1511.00561) [[Tutorial1]](http://mi.eng.cam.ac.uk/projects/segnet/tutorial.html) [[Tutorial2]](https://github.com/alexgkendall/SegNet-Tutorial)
- Multi-scale context aggregation by dilated convolutions [[Paper]](https://arxiv.org/pdf/1511.07122.pdf)

## 2016
- [**DeepLab v2**] DeepLab v2:Semantic Image Segmentation with Deep Convolutional Nets, Atrous Convolution, and Fully Connected CRFs** [[Project]](http://liangchiehchen.com/projects/DeepLab.html) [[Code-Caffe]](https://bitbucket.org/deeplab/deeplab-public/) [[Paper]](https://arxiv.org/abs/1606.00915)
- [**RefineNet**] [CVPR2017] RefineNet: Multi-Path Refinement Networks for High-Resolution Semantic Segmentation [[Code-MatConvNet]](https://github.com/guosheng/refinenet) [[Paper]](https://arxiv.org/abs/1611.06612)
- [**IFCN**] Improving Fully Convolution Network for Semantic Segmentation [[Paper]](https://arxiv.org/abs/1611.08986)
- [**FC-DenseNet**] [CVPRW2017] The One Hundred Layers Tiramisu: Fully Convolutional DenseNets for Semantic Segmentation [[Code-Theano]](https://github.com/SimJeg/FC-DenseNet) [[Code-Keras1]](https://github.com/titu1994/Fully-Connected-DenseNets-Semantic-Segmentation) [[Code-Keras2]](https://github.com/0bserver07/One-Hundred-Layers-Tiramisu) [[Paper]](https://arxiv.org/abs/1611.09326)
- [**PSPNet**] [CVPR2017] Pyramid Scene Parsing Network [[Project]](https://hszhao.github.io/projects/pspnet/) [[Code-Caffe]](https://github.com/hszhao/PSPNet) [[Paper]](https://arxiv.org/abs/1612.01105) [[Slides]](http://image-net.org/challenges/talks/2016/SenseCUSceneParsing.pdf)
- [**FusionNet**] FusionNet: A deep fully residual convolutional neural network for image segmentation in connectomics [[Code-PyTorch]](https://github.com/GunhoChoi/FusionNet_Pytorch) [[Paper]](https://arxiv.org/abs/1612.05360)

## 2017
- [**PixelNet**] PixelNet: Representation of the pixels, by the pixels, and for the pixels [[Project]](http://www.cs.cmu.edu/~aayushb/pixelNet/) [[Code-Caffe]](https://github.com/aayushbansal/PixelNet) [[Paper]](https://arxiv.org/abs/1702.06506)
- [**DUC-HDC**] [WACV 2018]Understanding Convolution for Semantic Segmentation [[Model-Mxnet]](https://drive.google.com/drive/folders/0B72xLTlRb0SoREhISlhibFZTRmM) [[Paper]](https://arxiv.org/abs/1702.08502) [[Code]](https://github.com/TuSimple/TuSimple-DUC)
- [**GCN**] [CVPR2017] Large Kernel Matters - Improve Semantic Segmentation by Global Convolutional Network [[Paper]](https://arxiv.org/abs/1703.02719)
- [CVPR 2017] Not All Pixels Are Equal: Difficulty-Aware Semantic Segmentation via Deep Layer Cascade-2017 [[Paper]](https://arxiv.org/abs/1704.01344)
- Pixel Deconvolutional Networks-2017 [[Code-Tensorflow]](https://github.com/HongyangGao/PixelDCN) [[Paper]](https://arxiv.org/abs/1705.06820)
- [**DRN**] [CVPR 2017] Dilated Residual Networks [[Paper]](https://arxiv.org/abs/1705.09914) [[Code]](https://github.com/fyu/drn)
- [**Deeplab v3**] Deeplab v3: Rethinking Atrous Convolution for Semantic Image Segmentation [[Paper]](https://arxiv.org/abs/1706.05587)
- [**LinkNet**] LinkNet: Exploiting Encoder Representations for Efficient Semantic Segmentation [[Paper]](https://arxiv.org/abs/1707.03718)
- [**SDN**] Stacked Deconvolutional Network for Semantic Segmentation [[Paper]](https://arxiv.org/pdf/1708.04943.pdf)
- Learning to Segment Every Thing [[Paper]](https://arxiv.org/pdf/1711.10370.pdf)

## 2018
- Panoptic Segmentation [[Paper]](https://arxiv.org/pdf/1801.00868.pdf)
- [**DeepLabv3+**] [ECCV 2018] Encoder-Decoder with Atrous Separable Convolution for Semantic Image Segmentation [[Paper]](https://arxiv.org/pdf/1802.02611.pdf) [[Code]](https://github.com/tensorflow/models/tree/master/research/deeplab)
- [**EncNet**] [CVPR 2018] Context Encoding for Semantic Segmentation [[Paper]](https://arxiv.org/abs/1803.08904) [[Code]](https://github.com/zhanghang1989/PyTorch-Encoding) (**Leverages global context to increase accuracy by adding a channel attention module, which triggers attention on certain feature maps based on a newly designed loss function. The loss is based on a network branch which predicts which classes are present in the image (i.e higher level global context)**)
- [ECCV 2018] Adaptive Affinity Fields for Semantic Segmentation [[Project]](https://jyhjinghwang.github.io/projects/aaf.html) [[Paper]](https://arxiv.org/abs/1803.10335) [[Code]](https://github.com/twke18/Adaptive_Affinity_Fields)
- [**EXFuse**] [ECCV 2018] ExFuse: Enhancing Feature Fusion for Semantic Segmentation [[Paper]](https://arxiv.org/abs/1804.03821) (**Uses deep supervision and explicitly combines the multi-scale features from the feature extraction frontend before processing, in order to ensure multi-scale information is processed together at all levels**)
- Vortex Pooling: Improving Context Representation in Semantic Segmentation [[Paper]](https://arxiv.org/abs/1804.06242)
- [**DFN**] [CVPR 2018] Learning a Discriminative Feature Network for Semantic Segmentation [[Paper]](https://arxiv.org/abs/1804.09337) (**Uses deep supervision and attempts to process the smooth and edge portions of the segments separately**)
- Stacked U-Nets: A No-Frills Approach to Natural Image Segmentation [[Paper]](https://arxiv.org/abs/1804.10343)
- [BMVC 2018] Pyramid Attention Network for Semantic Segmentation [[Paper]](https://arxiv.org/abs/1805.10180)
- [**G-FRNet**] [CVPR 2017] Gated Feedback Refinement Network for Coarse-to-Fine Dense Semantic Image Labeling [[Paper]](https://arxiv.org/abs/1806.11266) [[code]](https://github.com/mrochan/gfrnet)
- [CVPR 2018] Context Contrasted Feature and Gated Multi-Scale Aggregation for Scene Segmentation [[Paper]](http://openaccess.thecvf.com/content_cvpr_2018/html/Ding_Context_Contrasted_Feature_CVPR_2018_paper.html)
- [**DenseASPP**] [CVPR 2018] DenseASPP for Semantic Segmentation in Street Scenes [[Paper]](http://openaccess.thecvf.com/content_cvpr_2018/html/Yang_DenseASPP_for_Semantic_CVPR_2018_paper.html) [[code]](https://github.com/DeepMotionAIResearch/DenseASPP) (**Combines dense connections with atrous convolutions**)
- [CVPR 2018] Dense Decoder Shortcut Connections for Single-Pass Semantic Segmentation [[Paper]](http://openaccess.thecvf.com/content_cvpr_2018/html/Bilinski_Dense_Decoder_Shortcut_CVPR_2018_paper.html) (**Use dense connections in the decoding stage for higher accuracy (previously only done during feature extraction / encoding)**)
- Smoothed Dilated Convolutions for Improved Dense Prediction [[Paper]](https://arxiv.org/abs/1808.08931)
- [**PSANet**] [ECCV 2018] PSANet: Point-wise Spatial Attention Network for Scene Parsing [[Paper]](http://openaccess.thecvf.com/content_ECCV_2018/html/Hengshuang_Zhao_PSANet_Point-wise_Spatial_ECCV_2018_paper.html) [[project]](https://hszhao.github.io/projects/psanet/) [[code]](https://github.com/hszhao/PSANet) [[slide]](https://docs.google.com/presentation/d/1_brKNBtv8nVu_jOwFRGwVkEPAq8B8hEngBSQuZCWaZA/edit?usp=sharing) (<font color=red>Attention Mechanism</font>)
- [**OCNet**] OCNet: Object Context Network for Scene Parsing [[Paper]](https://arxiv.org/abs/1809.00916) [[code]](https://github.com/PkuRainBow/OCNet) (<font color=red>Attention Mechanism</font>)
- [**DAN**] [CVPR 2019] Dual Attention Network for Scene Segmentation [[Paper]](https://arxiv.org/abs/1809.02983) [[code]](https://github.com/junfu1115/DANet) (<font color=red>Attention Mechanism</font>)
- [**CCNet**] CCNet: Criss-Cross Attention for Semantic Segmentation [[Paper]](https://arxiv.org/abs/1811.11721) [[code]](https://github.com/speedinghzl/CCNet) (<font color=red>Attention Mechanism</font>)
- [**GloRe**] [CVPR 2019] Graph-Based Global Reasoning Networks [[Paper]](https://arxiv.org/abs/1811.12814) (<font color=red>Graph Convolution</font>)
- [**TKCN**] Tree-structured Kronecker Convolutional Networks for Semantic Segmentation [[Paper]](https://arxiv.org/abs/1812.04945) [[code]](https://github.com/wutianyiRosun/TKCN)  
- [**GCU**] Beyond Grids: Learning Graph Representations for Visual Recognition [[Paper]](https://papers.nips.cc/paper/8135-beyond-grids-learning-graph-representations-for-visual-recognition) (<font color=red>Graph Convolution</font>)

## 2019
- Auto-DeepLab: Hierarchical Neural Architecture Search for Semantic Image Segmentation[[Paper]](https://arxiv.org/abs/1901.02985)
- Decoders Matter for Semantic Segmentation: Data-Dependent Decoding Enables Flexible Feature Aggregation [[Paper]](https://arxiv.org/abs/1903.02120)
- [**CVPR 2019**] Structured Knowledge Distillation for Semantic Segmentation [[Paper]](https://arxiv.org/abs/1903.04197)
- [**CVPR 2019**] Knowledge Adaptation for Efficient Semantic Segmentation [[Paper]](https://arxiv.org/abs/1903.04688)
- [**CVPR 2019**] A Cross-Season Correspondence Dataset for Robust Semantic Segmentation [[Paper]](https://arxiv.org/abs/1903.06916)
- Efficient Smoothing of Dilated Convolutions for Image Segmentation [[Paper]](https://arxiv.org/abs/1903.07992) [[Code]](https://github.com/ThomasZiegler/Efficient-Smoothing-of-DilaBeyond GridsBeyond GridsBeyond GridsBeyondted-Convolutions)
- [**FastFCN**] FastFCN：Rethinking Dilated Convolution in the Backbone for Semantic Segmentation [[Paper]](https://arxiv.org/abs/1903.11816) [[Code]](https://github.com/wuhuikai/FastFCN)
- [**GFF**] GFF: Gated Fully Fusion for Semantic Segmentation [[Paper]](https://arxiv.org/abs/1904.01803)
- DADA: Depth-aware Domain Adaptation in Semantic Segmentation [[Paper]](https://arxiv.org/abs/1904.01886)
- [**HRNetV2**] High-Resolution Representations for Labeling Pixels and Regions [[Paper]](https://arxiv.org/abs/1904.04514)

# Real-Time Semantic Segmentation
1. [**ENet**] ENet: A Deep Neural Network Architecture for Real-Time Semantic Segmentation-2016  [[Paper]](https://arxiv.org/abs/1606.02147)
2. [**ICNet**] [ECCV 2018] ICNet for Real-Time Semantic Segmentation on High-Resolution Images [[Project]](https://hszhao.github.io/projects/icnet/) [[Code]](https://github.com/hszhao/ICNet) [[Paper]](https://arxiv.org/abs/1704.08545) [[Video]](https://www.youtube.com/watch?v=qWl9idsCuLQ) (**Uses deep supervision and runs the input image at different scales, each scale through their own subnetwork and progressively combining the results**)
3. [**RTSeg**] RTSeg: Real-time Semantic Segmentation Comparative Study [[Paper]](https://arxiv.org/abs/1803.02758)
4. [**ShuffleSeg**] ShuffleSeg: Real-time Semantic Segmentation Network [[Paper]](https://arxiv.org/abs/1803.03816)
5. [**ESPNet**] [ECCV 2018] ESPNet: Efficient Spatial Pyramid of Dilated Convolutions for Semantic Segmentation [[Paper]](https://arxiv.org/pdf/1803.06815.pdf)
6. [**ContextNet**] [BMVC 2018] ContextNet: Exploring Context and Detail for Semantic Segmentation in Real-time [[Paper]](https://arxiv.org/abs/1805.04554)
7. Guided Upsampling Network for Real-Time Semantic Segmentation [[Project]](http://www.ivl.disco.unimib.it/activities/semantic-segmentation/) [[Paper]](https://arxiv.org/abs/1807.07466)
8. [**BiSeNet**] [ECCV 2018] BiSeNet: Bilateral Segmentation Network for Real-time Semantic Segmentation [[Paper]](https://arxiv.org/abs/1808.00897) (**Has 2 branches: one is deep for getting semantic information, while the other does very little / minor processing on the input image as to preserve the low-level pixel information**)
9. Efficient Dense Modules of Asymmetric Convolution for Real-Time Semantic Segmentation [[Paper]](https://arxiv.org/abs/1809.06323)
10. [BMVC 2018] Light-Weight RefineNet for Real-Time Semantic Segmentation [[Paper]](https://arxiv.org/abs/1810.03272) [[code]](https://github.com/DrSleep/light-weight-refinenet)
11. CGNet: A Light-weight Context Guided Network for Semantic Segmentation [[Paper]](https://arxiv.org/abs/1811.08201) [[Code]](https://github.com/wutianyiRosun/CGNet) 
12. ~~ShelfNet for Real-time Semantic Segmentation [[Paper]](https://arxiv.org/abs/1811.11254)~~
13. ESPNetv2: A Light-weight, Power Efficient, and General Purpose Convolutional Neural Network [[Paper]](https://arxiv.org/abs/1811.11431)[[Code]](https://github.com/sacmehta/ESPNetv2) 
14. Real time backbone for semantic segmentation [[Paper]](https://arxiv.org/abs/1903.06922)
15. DSNet for Real-Time Driving Scene Semantic Segmentation [[Paper]](https://arxiv.org/abs/1812.07049)
16. In Defense of Pre-trained ImageNet Architectures for Real-time Semantic Segmentation of Road-driving Images [[Paper]](https://arxiv.org/abs/1903.08469)
17. Residual Pyramid Learning for Single-Shot Semantic Segmentation [[Paper]](https://arxiv.org/abs/1903.09746)
18. DFANet: Deep Feature Aggregation for Real-Time Semantic Segmentation [[Paper]](https://arxiv.org/abs/1904.02216)

# Loss Fuction
1. <font color=red>The Lovász Hinge: A Novel Convex Surrogate for Submodular Losses</font> [[arxiv]](https://arxiv.org/abs/1512.07797) [[project]](https://sites.google.com/site/jiaqianyu08/lovaszhinge)
2. [CVPR 2017 ] Loss Max-Pooling for Semantic Image Segmentation [[Paper]](https://arxiv.org/abs/1704.02966)
3. [CVPR 2018] <font color=red>The Lovász-Softmax loss：A tractable surrogate for the optimization of the intersection-over-union measure in neural networks</font> [[Project]](http://bmax.im/LovaszSoftmax) [[Paper]](https://arxiv.org/abs/1705.08790) [[Code]](https://github.com/bermanmaxim/LovaszSoftmax)
4. Generalised Dice overlap as a deep learning loss function for highly unbalanced segmentations [[Paper]](https://arxiv.org/abs/1707.03237)
5. <font color=red>IoU is not submodular</font> [[arxiv]](https://arxiv.org/abs/1809.00593)
6. <font color=red>Yes, IoU loss is submodular - as a function of the mispredictions</font> [[arxiv]](https://arxiv.org/abs/1809.01845)
7. [BMVC 2018] NeuroIoU: Learning a Surrogate Loss for Semantic Segmentation [[Paper]](http://cdn.iiit.ac.in/cdn/cvit.iiit.ac.in/images/ConferencePapers/2018/bmvc2018-NeuroIoU.pdf) [[code]](https://github.com/drsleep/light-weight-refinenet)


# Review
- A Survey of Semantic Segmentation [[arxiv]](https://arxiv.org/abs/1602.06541)
- A Review on Deep Learning Techniques Applied to Semantic Segmentation [[arxiv]](https://arxiv.org/abs/1704.06857)
- Recent progress in semantic image segmentation [[arxiv]](https://arxiv.org/abs/1809.10198)
