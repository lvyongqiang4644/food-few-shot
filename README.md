  Few-Shot Food Recognition via Multi-View Representation Learning
====
  Description
--
  In this paper, we have proposed a Multi-View Few-Shot Learning (MVFSL) framework to explore additional ingredient information for few-shot food recognition. In order to take advantage of ingredient information, These two kinds of features are effectively by first combining their extracted feature maps from the last convolution layer of their respective fine-tuned deep networks, and then conducting the convolution on the combined feature maps. In addition, this convolution is incorporated into a multi-view relation network, which is used to compare query images against labeled samples to obtain the image-level relation score.

Experimental Evaluation for  MVFSL
--
Model| Food-101| VIREO Food-172|ChineseFoodNet
:-----:|:-----:|:-----:|:----------:|
RN-Category | 53.9%|74.0%| 63.8%| 
RN-Ingredeint| 53.5%|70.5%|64.0%|
MVFSL-LC|55.1%|74.8%|65.8%|
**MVFSL-TC**|**55.3%**|**75.1%**|**66.1%**|
## Split&Pre-trained models
[split.zip](https://www.baidu.com/)  contains the train/test split of three food datasets(Food-101,VIREO Food172 and ChineseFoodNet) used in our paper. we show the category split, also the ingredient split. 
[Pre-trained_model](https://www.baidu.com/) contains all the pre-trained models in this work.
## Requirements
Training and testing codes are integrated into one repositories:
- tensorflow 1.x
- python 3.x
#### train&test
For MVFSL-TC:
```
$ python MVFSL-TC/MVFSL-TC_train.py
```
Note: The model need to be initialized by pre-trained model, and you need to modify the path.  
For MVFSL-LC:
```
$ python MVFSL-LC/MVFSL-LC_train.py
```
