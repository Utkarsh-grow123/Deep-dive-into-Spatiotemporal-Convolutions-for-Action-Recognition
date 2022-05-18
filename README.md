# Deep-dive-into-Spatiotemporal-Convolutions-for-Action-Recognition

This is the PyTorch implementation : **Deep-dive-into-Spatiotemporal-Convolutions-for-Action-Recognition**.

In this paper, we propose an improved R(2+3)D architecture that is superior to the pre-existing versions for the UCF101 dataset. We have also proposed a new network design for harnessing the potential efficacy and modelling flexibility of spatiotemporal convolutions by performing an empirical study on the effects of various spatiotemporal convolutions for action recognition in videos. We have used R(2+3)D ResNet architecure. Our test accuracy was 86.88% as compared to 73.5% accuracy as mentioned in the paper. This is due to the addition of visual image transformers in our main architecture.. 


## Data preparation

### UCF101

Download the UCF101 Dataset in form of frames from [here]([http://image-net.org/]([https://www.kaggle.com/datasets/pevogam/ucf101-frames?resource=download](https://www.kaggle.com/datasets/pevogam/ucf101-frames?resource=download))),

```

This dataset takes about one week to train, for efficiency, we have added our pre-trained model weights here.



## Results on ImageNet

### Main Results

| Method           | Pre-trained | UCF101 Accuracy     |                                                                                                     |
| -------------- | --------- | ---------- | -------------- | -------------- | 
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








