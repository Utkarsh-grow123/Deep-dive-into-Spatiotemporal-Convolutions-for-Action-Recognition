# Deep-dive-into-Spatiotemporal-Convolutions-for-Action-Recognition

Welcome to the Final Project for Deep Learning ECE-GY 7123. This project was done by 
* Utkarsh Grover ug2018@nyu.edu 
* Abirami Ravishankar ar7115@nyu.edu 

This is the PyTorch implementation : **Deep-dive-into-Spatiotemporal-Convolutions-for-Action-Recognition**.

tl;dr

In this paper, we propose an improved R(2+3)D architecture that is superior to the pre-existing versions for the UCF101 dataset which use R(2+1)D architecture. We have also proposed a new network design for harnessing the potential efficacy and modelling flexibility of spatiotemporal convolutions by performing an empirical study on the effects of various spatiotemporal convolutions for action recognition in videos. We have used R(2+3)D ResNet architecure. Our test accuracy was 86.88% as compared to 73.5% accuracy as mentioned in the paper. R(2+1)D outperforms I3D by 4.5% when trained from scratch on RGB, whereas our model R(3+2)D outperforms R(2+1)D by 11.4% trained from scratch. R(2+3)D pre-trained on kinetics400, out-performs R(2+1)D pre-trained on Sports-1M and I3D pre-trained on ImageNet, for both RGB. 


## Data preparation

### UCF101

Download the UCF101 Dataset in form of frames from [here](https://www.kaggle.com/datasets/pevogam/ucf101-frames?resource=download)


Caution: This dataset takes about one week to train, for efficiency, we have added our pre-trained model weights here. We have also attached our results to view directly.

Data folder for data augmentation
Models is for the model we used and pre-existing model for comparison


### Key Results

| Method           | Pre-trained | UCF101 Accuracy                                                        | Log                                                          |
| -------------- | --------- | ---------- | -------------- | -------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| I3D-RGB             | none          | 67.5     |
| I3D-RGB             | image-net     | 72.5     |
| I3D-FLOW            | image-net     | 65.3     |
| I3D-TWO STREAM      | image-net     | 75.7     |
| R(2+1)D-RGB         | none          | 75.7     |
| R(2+1)D-FLOW        | none          | 67.5     |
| R(2+1)D-TWO STREAM  | none          | 73.9     |
| R(2+1)D-RGB         | Sports-1M     | 74.3     |
| R(2+1)D-FLOW        | Sports-1M     | 68.5     |
| R(2+1)D-TWO STREAM  | Sports-1M     | 75.4     |
| R(2+3)D-RGB         | Kinetics-400  | 86.8     |
