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

## Getting Started:
### Usage
1. Clone this github repo. 
```
git clone https://github.com/Joannechiao18/Improved-GANomaly.git
```
2. Please `cd` to the `Improved-GANomaly-main`, and run the file `GANomaly_copy.ipynb` in Google Colab.

## Results:
We evaluated our results over three baseline models: `AnoGAN`, `EGBAD`, and `the original GANomaly` on the mvtec testing datasets. 
1. The results are as the following: 
| Column 1 Header | Column 2 Header | Column 3 Header |
| --------------- | --------------- | --------------- |
| Row 1 Column 1 | Row 1 Column 2 | Row 1 Column 3 |
| Row 2 Column 1 | Row 2 Column 2 | Row 2 Column 3 |
| Row 3 Column 1 | Row 3 Column 2 | Row 3 Column 3 |

