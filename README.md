# Hybrid CNN-Swin
This is a TensorFlow and Keras-based implementation of Hybrid CNN-Swin in the 12th ISCTech paper "A Hybrid CNN-Swin Transformer Module for Hyperspectral Image Classification".

Paper links: [CNN-Swin published on 12th International Conference on Information Systems and Computing Technology (ISCTech)] 
(https://ieeexplore.ieee.org/abstract/document/10845311)

The Paiva University and Salinas datasets can be downloaded from  (https://www.ehu.eus/ccwintco/index.php/Hyperspectral_Remote_Sensing_Scenes#Pavia_Centre_and_University)

## Description 
The hybrid CNN-Swin Transformer Module presents a novel approach integrating the strengths of both 3D and 2D convolutional neural networks (CNNs) and the Swin Transformer for robust HSI classification. The 3D-CNN leverages the inherent three-dimensional structure of HSIs to capture intricate spectral-spatial features, which are crucial for accurate classification, and the 2D-CNN to know more about spatial representation. The Swin Transformer, with its group attention and sliding window mechanisms, effectively learns long-range spectral dependencies while preserving global information to improve the representation of features. The calculation of sliding window attention can consider the contextual information of various windows, which is to be able to keep the global features of the HSI and enhance the outcomes of classification.


## Model
<img src="Figures/Figure 1.jpg"/>
Figure 1. Overall structure of the proposed model for HSI classification.

In our model, we divided all datasets into 30% for the training set and the remaining 70% for the testing set.

#### Note: In our code, it can change the dataset division to be suitable to compare with any method that uses different division


## Prerequisites
- [Anaconda 4.9.2](https://www.anaconda.com/download)
- [Tensorflow 2.10.1](https://github.com/tensorflow/tensorflow/tree/r2.10)
- [Keras 2.10.0](https://github.com/fchollet/keras)

## Results

### Indian Pines (IP) dataset

<img src="Figures/Fig. 4.jpg"/> 
Figure 2.   Comparison of classification maps between various models on the IP dataset.

### Salinas Scene (SA) dataset

<img src="Figures/Fig. 5.jpg"/> 
Figure 2.   Comparison of classification maps between various models on the SA dataset.

### University of Pavia (UP) dataset

<img src="Figures/Fig. 6.jpg"/> 
Figure 2.   Comparison of classification maps between various models on the PU dataset.

## Thanks
1. https://github.com/microsoft/Swin-Transformer
2. https://github.com/MinatoRyu007/Swin-HSI
3. https://github.com/Pancakerr/HybridSN

## Acknowledgement
We encourage researchers to cite our work.

We encourage researchers to conduct different comparative experiments (papers) within a code framework to ensure a fair comparison.

If you encounter any problems reproducing the code, please do not hesitate to contact us.

Email: mosahaidarh@stu.xidian.edu.cn, mosa.haidarh@taiz.edu.ye
