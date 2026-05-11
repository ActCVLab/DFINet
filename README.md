## DFINet: Dynamic feedback iterative network for infrared small target detection
Paper: https://www.sciencedirect.com/science/article/abs/pii/S0031320325006181
## Contributions
1.We innovatively introduce an iterative feedback mechanism in IRSTD and propose DFINet to facilitate feature learning during training and implement error correction during inference.

2.In order to guide the model to focus on key regions and reduce error accumulation, the DFFFM is devised to achieve dynamic information interaction with HPMK.

3.In order to effectively aggregate high-level and low-level features, a novel feedback-based cross-layer feature fusion module DSFM is proposed.
## Framework of DFINet
(https://github.com/uisdu/DFINet/blob/main/Fig/framework.png)
## Visual
(https://github.com/uisdu/DFINet/blob/main/Fig/iter.png)
## Train
To train DFINet from scratch, run:
```
python train.py
```
## Test
Training logs and checkpoints are available at:
## 百度网盘权重文件：[权重文件](https://pan.baidu.com/share/init?surl=Hqis60HFyzqIJ7dgC4A-Qg) 提取密码:9qy7
This code is highly borrowed from [FANet](https://github.com/nikhilroxtomar/FANet). Thanks to Nikhil Kumar Tomar.

This code is highly borrowed from [IRSTD-Toolbox](https://github.com/XinyiYing/BasicIRSTD). Thanks to Xinyi Ying.

## Citation
If you use this code, please kindly cite our paper:
```
@article{WU2026111958,
title = {DFINet: Dynamic feedback iterative network for infrared small target detection},
journal = {Pattern Recognition},
volume = {169},
pages = {111958},
year = {2026},
issn = {0031-3203},
doi = {https://doi.org/10.1016/j.patcog.2025.111958},
url = {https://www.sciencedirect.com/science/article/pii/S0031320325006181},
author = {Jing Wu and Changhai Luo and Zhaobing Qiu and Liqiong Chen and Rixiang Ni and Yunxiang Li and Feng Huang and Jian Wu},
keywords = {Feedback iteration, Infrared small target detection, Feature mining, Error correction},
abstract = {Recently, deep learning-based methods have made impressive progress in infrared small target detection (IRSTD). However, the weak and variable nature of small targets constrains the feature extraction and scene adaptation of existing methods, leading to low data utilization and poor robustness. To address this issue, we innovatively introduce the feedback mechanism into IRSTD and propose the dynamic feedback iterative network (DFINet). The main motivation is to guide the model training and prediction utilizing the history prediction mask (HPMK) of previous rounds. On the one hand, in the training phase, DFINet can further mine the key features of real targets by training in multiple iterations with limited data; on the other hand, in the prediction phase, DFINet can correct the wrong results through feedback iterative to improve the model robustness. Specifically, we first propose the dynamic feedback feature fusion module (DFFFM), which dynamically interacts HPMK with feature maps through a hard attention mechanism to guide feature mining and error correction. Then, for better feature extraction, the cascaded hybrid pyramid pooling module (CHPP) is devised to capture both global and local information. Finally, we propose the dynamic semantic fusion module (DSFM), which innovatively utilizes feedback information to guide the fusion of high-level and low-level features for better feature representation in different scenarios. Extensive experimental results on publicly available datasets of NUDT-SIRST, IRSTD-1k, and SIRST Aug show that DFINet outperforms several state-of-the-art methods and achieves superior detection performance. Our code will be publicly available at https://github.com/uisdu/DFINet.}
}
```
## Contact
If you have any questions, please contact:  
Author: Zhaobing Qiu  
Email: qiuzhaobing@fzu.edu.cn  
Copyright: Fuzhou University 
## License
This code is only freely available for non-commercial research use.

If you find some help for you, star is a good reward ^_^. 
