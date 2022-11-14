# Improved-GANomaly

![](https://img.shields.io/badge/tensorflow-1.9.1-yellow)
![](https://img.shields.io/badge/Cuda-10.2-blue)


This is an improved version GANomaly with keras from YZU graduate-level course Machine Learning class. 

## Introduction 
To overcome the challenge that the original GANomaly had already learned many tiny features of images, which is hard to make further improvements. I revisited the principle paper "GANomaly: Semi-Supervised Anomaly Detection via Adversarial Training" and learned that anomaly score definition in the inferencing stage is crucial. Therefore, I re-defined a new anomaly score, aiming to calculate differences between features from generated and testing images by the encoder trained on regular samples.

### Dependencies
* tensorflow 
* sklearn 
* time 
* matplotlib 
* pytorch 
* random 
* cv2 
* os 
* glob 
* numpy 

### Dataset
* The anomaly detection dataset for training G2 can be downloaded from [here]([https://www.robots.ox.ac.uk/~vgg/data/flowers/102/](https://www.mvtec.com/company/research/datasets/mvtec-ad)).

### It was tested and runs under the following OSs:
* Windows 10
* Linux 

## Getting Started:
### Usage
1. Clone this github repo. 
```
git clone https://github.com/bigmms/DualGAN
```
