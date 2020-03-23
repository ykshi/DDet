# DDet

[DDet: Dual-path Dynamic Enhancement Network for Real-World Image Super-Resolution](https://arxiv.org/abs/2002.11079)(DDet), IEEE SPL 2020.

# Prerequisites
- Computer with Linux 16.04
- Caffe
- Matcaffe

# Installation
Our work requires the [kernel predication layer](https://github.com/csjcai/RealSR)(KPL). Hence, we need to add KPL into caffe.
1. Download the new layers in folder ['Layer'](https://github.com/csjcai/RealSR/tree/master/Layer).
2. Modify the default caffe.proto with [caffe.proto](https://github.com/ykshi/DDet/blob/master/caffe.proto).
3. Compile whole caffe project.

# Dataset
We conduct [version2](https://drive.google.com/open?id=1dEBRo_1HH6Yk9zrchEg_JTRi-Uhmd-sj) of [RealSR dataset](https://github.com/csjcai/RealSR) as default dataset. 

According to the official setting, we use 459 scenes for training and the rest 100 scenes are adopted for testing. Moreover, other versions of RealSR dataset or other non-inherently aligned image pair is fine for our model.

# Models
We upload the [2x](https://github.com/ykshi/DDet/tree/master/x2), [3x](https://github.com/ykshi/DDet/tree/master/x3) and [4x](https://github.com/ykshi/DDet/tree/master/x4) models and corresponding prototxt for evaluation. These models will certainly fine for other domain data as long as some finetune metric is incorporated.
Besides, Matcaffe is required for testing, a concise matcaffe test demo is demonstrated in [here](https://github.com/csjcai/RealSR/blob/master/Test/Test.m).

# Results

<div align="center">
        <img src="https://github.com/ykshi/DDet/blob/master/png/demo.png"/>
        <img src="https://github.com/ykshi/DDet/blob/master/png/results.png"/>
</div>

#Feedback and Citation
``
@article{shi2020ddet,
  title={DDet: Dual-path Dynamic Enhancement Network for Real-World Image Super-Resolution},
  author={Shi, Yukai and Zhong, Haoyu and Yang, Zhijing and Yang, Xiaojun and Lin, Liang},
  journal={arXiv preprint arXiv:2002.11079},
  year={2020}
}
``
if you have any question, please feel free to contact me by sending mail to `ykshi.1991ATfoxmail.com`.


# Acknowledgement
This code is heavily rely on [RealSR framework](https://github.com/csjcai/RealSR), thanks for their great effort.
