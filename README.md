# Deep-dive-into-Spatiotemporal-Convolutions-for-Action-Recognition

Welcome to the Final Project for Deep Learning ECE-GY 7123. This project was done by 
* Utkarsh Grover ug2018@nyu.edu 
* Abirami Ravishankar ar7115@nyu.edu 


## tl;dr

In this paper, we propose an improved R(2+3)D architecture that is superior to the pre-existing versions for the UCF101 dataset which use R(2+1)D architecture. We have also proposed a new network design for harnessing the potential efficacy and modelling flexibility of spatiotemporal convolutions by performing an empirical study on the effects of various spatiotemporal convolutions for action recognition in videos. We have used R(2+3)D ResNet architecure. R(2+1)D outperforms I3D by 4.5% when trained from scratch on RGB, whereas our model R(3+2)D outperforms R(2+1)D by 11.4% trained from scratch. R(2+3)D pre-trained on kinetics400, out-performs R(2+1)D pre-trained on Sports-1M and I3D pre-trained on ImageNet, for both RGB. Our test accuracy was 86.88% as compared to 73.5% accuracy as mentioned in the paper.

## Implementation

### UCF101

Download the UCF101 Dataset in form of frames from [here](https://www.kaggle.com/datasets/pevogam/ucf101-frames?resource=download)


Caution: This dataset takes about one week to train, for efficiency, we have added our pre-trained model weights here. We have also attached our results to view directly.

 data : Data folder for data augmentation
 Models : Models folder is for the model R(2+1)D and R(3+2)D 
 
 
 slurm-30949.out : This is the .out file that has a vivid description of results of our code. This is done because this model takes weeks to pre-train on Kinetic dataset and then test on UCF101. Hence we have uploaded this file for easy understanding of our proceedings.

This is a PyTorch implementation.


## Result 

![alt text](https://github.com/Utkarsh-grow123/Deep-dive-into-Spatiotemporal-Convolutions-for-Action-Recognition/blob/main/Table.png)
