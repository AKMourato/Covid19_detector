# Detecting COVID-19 from Chest X-Ray images

In this repository is an implementation of a classification model for detection of COVID-19 from Chest X-Rays in Pytorch.

The dataset used is provided. The data distribution followed:

|  Type | Normal | Viral Pneumonia | COVID-19 | Total |
|:-----:|:------:|:--------:|:--------:|:-----:|
| Train | 1311 | 1315 | 1113 | 3739 |
|  Test |  30 | 30 | 30 | 90 |

<p align="left">
  <img src="https://github.com/MKSK22/Detecting_Covid19_fromChestXrays/blob/main/covid_samples.png"/>
</p>

### Model
It was used a pre-trained Resnet-18 model on ImageNet. Transfer learning was applied, replacing the standard fully convolutional layer with 1000 output features to just 3, according to the three types of cases.

For aditional info check the notebook.

<p align="center">
  <img src="https://github.com/MKSK22/Detecting_Covid19_fromChestXrays/blob/main/resnet18.png"/>
</p>

### Results

The model reach a 95% accuracy in the test phase.

<p align="center">
  <img src="https://github.com/MKSK22/Detecting_Covid19_fromChestXrays/blob/main/pred.png"/>
</p>

<p align="center">
  <img src="https://github.com/MKSK22/Detecting_Covid19_fromChestXrays/blob/main/pred2.png"/>
</p>
