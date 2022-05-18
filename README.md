# Deep-dive-into-Spatiotemporal-Convolutions-for-Action-Recognition

This is the PyTorch implementation : **Deep-dive-into-Spatiotemporal-Convolutions-for-Action-Recognition**.

In this paper, we propose an improved R(2+3)D architecture that is superior to the pre-existing versions for the UCF101 dataset. We have also proposed a new network design for harnessing the potential efficacy and modelling flexibility of spatiotemporal convolutions by performing an empirical study on the effects of various spatiotemporal convolutions for action recognition in videos. We have used R(2+3)D ResNet architecure. Our test accuracy was 86.88% as compared to 73.5% accuracy as mentioned in the paper. This is due to the addition of visual image transformers in our main architecture.. 


## Data preparation

### UCF101

Download the UCF101 Dataset in form of frames from [here]([http://image-net.org/](https://www.kaggle.com/datasets/pevogam/ucf101-frames?resource=download)),

```
This Dayaset take around one week of training hence we have put out pre-trained model weights here for anyone to use








## Results on ImageNet

### Main Results

| Method           | Pre-trained | UCF101 Accuracy     |                                                                                                     |
| -------------- | --------- | ---------- | -------------- | -------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| I3D-RGB             | none          | 67.5     |
| I3D-RGB             | image-net     | 67.5     |
| I3D-FLOW            | image-net     | 67.5     |
| I3D-TWO STREAM      | image-net     | 67.5     |
| R(2+1)D-RGB         | none          | 67.5     |
| R(2+1)D-FLOW        | none          | 67.5     |
| R(2+1)D-TWO STREAM  | none          | 67.5     |
| R(2+1)D-RGB         | Sports-1M     | 67.5     |
| R(2+1)D-FLOW        | Sports-1M     | 67.5     |
| R(2+1)D-TWO STREAM  | Sports-1M     | 67.5     |
| R(2+3)D-RGB         | none          | 67.5     |








