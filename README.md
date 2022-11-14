# Improved-GANomaly

![](https://img.shields.io/badge/tensorflow-1.9.1-yellow)
![](https://img.shields.io/badge/Cuda-10.2-blue)


This is an improved version GANomaly with keras from YZU graduate-level course Machine Learning class. 

## Introduction 
To overcome the challenge that the original GANomaly had already learned many tiny features of images, which is hard to make further improvements, I revisited the principle paper "GANomaly: Semi-Supervised Anomaly Detection via Adversarial Training" and then re-defined a new anomaly score, which calculates the differences between features from generated and testing images by the encoder trained on regular samples.

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
1. The results after comparing our improved GANomaly with AnoGAN and EGBAD: 

|                 | AnoGAN          | EGBAD           | Ours           |
| --------------- | --------------- | --------------- | ---------------|
| Accuracy        | 70.8 %          | 74.7 %          | 83.8 %         |
| F1-Score        | 67.6 %          | 85.5 %          | 89.0 %         |
| Inference Time  | 827.3 s         | 101.5 s         | 11.9 s         |



|                 | Original GANomaly                 |Ours                              ||
| --------------- | --------------- | --------------- | --------------- | --------------- |
|                 | Accuracy        | F1-Score        | Accuracy        | F1-Score        |
| Accuracy        | 70.8 %          | 74.7 %          | 70.8 %          | 74.7 %          |
| F1-Score        | 67.6 %          | 85.5 %          | 70.8 %          | 74.7 %          |

