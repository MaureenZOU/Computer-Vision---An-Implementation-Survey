# What-could-Deep-Learning-do

Explore Top Researchers' work, get the fowllowing information:
* An experiment base Problem Setting (Input, Output)
* Model Structure
* Network Structure
* Dataset Scale
* Data Augmentation
* Initialization and Optimization

## Kaiming He
### [Deep Residual Learning for Image Recognition](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/He_Deep_Residual_Learning_CVPR_2016_paper.pdf)

#### Problem Setting
* ImageNet Classification
* Cifar 10
* Object Detection on PASCAL and MS COCO

#### Model Structure
A general Encoder structure
#### Network Structure
![alt text](https://github.com/MaureenZOU/What-could-Deep-Learning-do/blob/master/imgs/resnet.png)
![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `why the channel size first increase and decrease like 256 - 1024 - 512`

# Dataset Scale
1.28 million train, 50k validation, 100k test images (ImageNet)


# Data Augmentation
* Scale Augmentation \[256, 480\] [ref](https://arxiv.org/pdf/1409.1556.pdf)
* Flipping (left and right flip)
* Random Crop (224)
* Mean subtraction (per pixel)
* Standard color augmentation [ref](https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf)
* Batch Normalization after each convolution before activation

# Initialization and Optimization
* Kaiming Initialization
* SGD  lr = 0.1, divided by 10 when the error plateaus, weight decay of 0.0001, a momentum of 0.9
* 60 × 10^4 iterations


