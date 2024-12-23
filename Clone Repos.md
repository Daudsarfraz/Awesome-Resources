import re

# The list of Awesome Lists as a string
awesome_lists = """
- [Awesome Machine Learning](https://github.com/josephmisiti/awesome-machine-learning)
- [Awesome Deep Vision](https://github.com/kjw0612/awesome-deep-vision)
- [Awesome Domain Adaptation](https://github.com/zhaoxin94/awesome-domain-adaptation)
- [Awesome Object Detection](https://github.com/amusi/awesome-object-detection)
- [Awesome 3D Machine Learning](https://github.com/timzhang642/3D-Machine-Learning)
- [Awesome Action Recognition](https://github.com/jinwchoi/awesome-action-recognition)
- [Awesome Scene Understanding](https://github.com/bertjiazheng/awesome-scene-understanding)
- [Awesome Adversarial Machine Learning](https://github.com/yenchenlin/awesome-adversarial-machine-learning)
- [Awesome Adversarial Deep Learning](https://github.com/chbrian/awesome-adversarial-examples-dl)
- [Awesome Face](https://github.com/polarisZhao/awesome-face)
- [Awesome Face Recognition](https://github.com/ChanChiChoi/awesome-Face_Recognition)
- [Awesome Human Pose Estimation](https://github.com/wangzheallen/awesome-human-pose-estimation)
- [Awesome medical imaging](https://github.com/fepegar/awesome-medical-imaging)
- [Awesome Images](https://github.com/heyalexej/awesome-images)
- [Awesome Graphics](https://github.com/ericjang/awesome-graphics)
- [Awesome Neural Radiance Fields](https://github.com/yenchenlin/awesome-NeRF)
- [Awesome Implicit Neural Representations](https://github.com/vsitzmann/awesome-implicit-representations)
- [Awesome Neural Rendering](https://github.com/weihaox/awesome-neural-rendering)
- [Awesome Public Datasets](https://github.com/awesomedata/awesome-public-datasets)
- [Awesome Dataset Tools](https://github.com/jsbroks/awesome-dataset-tools)
- [Awesome Robotics Datasets](https://github.com/sunglok/awesome-robotics-datasets)
- [Awesome Mobile Machine Learning](https://github.com/fritzlabs/Awesome-Mobile-Machine-Learning)
- [Awesome Explainable AI](https://github.com/wangyongjie-ntu/Awesome-explainable-AI)
- [Awesome Fairness in AI](https://github.com/datamllab/awesome-fairness-in-ai)
- [Awesome Machine Learning Interpretability](https://github.com/jphall663/awesome-machine-learning-interpretability)
- [Awesome Production Machine Learning](https://github.com/EthicalML/awesome-production-machine-learning)
- [Awesome Video Text Retrieval](https://github.com/danieljf24/awesome-video-text-retrieval)
- [Awesome Image-to-Image Translation](https://github.com/weihaox/awesome-image-translation)
- [Awesome Image Inpainting](https://github.com/1900zyh/Awesome-Image-Inpainting)
- [Awesome Deep HDR](https://github.com/vinthony/awesome-deep-hdr)
- [Awesome Video Generation](https://github.com/matthewvowels1/Awesome-Video-Generation)
- [Awesome GAN applications](https://github.com/nashory/gans-awesome-applications)
- [Awesome Generative Modeling](https://github.com/zhoubolei/awesome-generative-modeling)
- [Awesome Image Classification](https://github.com/weiaicunzai/awesome-image-classification)
- [Awesome Deep Learning](https://github.com/ChristosChristofidis/awesome-deep-learning)
- [Awesome Machine Learning in Biomedical(Healthcare) Imaging](https://github.com/XindiWu/Awesome-Machine-Learning-in-Biomedical-Healthcare-Imaging)
- [Awesome Deep Learning for Tracking and Detection](https://github.com/abhineet123/Deep-Learning-for-Tracking-and-Detection)
- [Awesome Human Pose Estimation](https://github.com/wangzheallen/awesome-human-pose-estimation)
- [Awesome Deep Learning for Video Analysis](https://github.com/HuaizhengZhang/Awsome-Deep-Learning-for-Video-Analysis)
- [Awesome Vision + Language](https://github.com/yuewang-cuhk/awesome-vision-language-pretraining-papers)
- [Awesome Robotics](https://github.com/kiloreux/awesome-robotics)
- [Awesome Visual Transformer](https://github.com/dk-liang/Awesome-Visual-Transformer)
- [Awesome Embodied Vision](https://github.com/ChanganVR/awesome-embodied-vision)
- [Awesome Anomaly Detection](https://github.com/hoya012/awesome-anomaly-detection)
- [Awesome Makeup Transfer](https://github.com/thaoshibe/awesome-makeup-transfer)
- [Awesome Learning with Label Noise](https://github.com/subeeshvasu/Awesome-Learning-with-Label-Noise)
- [Awesome Deblurring](https://github.com/subeeshvasu/Awesome-Deblurring)
- [Awsome Deep Geometry Learning](https://github.com/subeeshvasu/Awsome_Deep_Geometry_Learning)
- [Awesome Image Distortion Correction](https://github.com/subeeshvasu/Awesome-Image-Distortion-Correction)
- [Awesome Neuron Segmentation in EM Images](https://github.com/subeeshvasu/Awesome-Neuron-Segmentation-in-EM-Images)
- [Awsome Delineation](https://github.com/subeeshvasu/Awsome_Delineation)
- [Awesome ImageHarmonization](https://github.com/subeeshvasu/Awesome-ImageHarmonization)
- [Awsome GAN Training](https://github.com/subeeshvasu/Awesome-GAN-Training)
- [Awesome Document Understanding](https://github.com/tstanislawek/awesome-document-understanding)
"""

# Regular expression to find all GitHub repository links
repo_links = re.findall(r'https://github.com/[^\s]+', awesome_lists)

# Store the links in a text file
with open("github_links.txt", "w") as file:
    for link in repo_links:
        file.write(link + "\n")

print("Links have been saved to github_links.txt")


for repo in $(cat github_links.txt); do git clone $repo; done

write this command to clone all reposs from Internet
