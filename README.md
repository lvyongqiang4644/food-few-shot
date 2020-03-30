  Few-Shot Food Recognition via Multi-View Representation Learning
====
  Description
--
  In this paper, we have proposed a Multi-View Few-Shot Learning (MVFSL) framework to explore additional ingredient information for few-shot food recognition. In order to take advantage of ingredient information, These two kinds of features are effectively by first combining their extracted feature maps from the last convolution layer of their respective fine-tuned deep networks, and then conducting the convolution on the combined feature maps. In addition, this convolution is incorporated into a multi-view relation network, which is used to compare query images against labeled samples to obtain the image-level relation score.

Experimental Evaluation for  MVFSL
--
Model| Food-101| VIREO Food-172|ChineseFoodNet
:-----:|:-----:|:-----:|:----------:|
RN-Category | 53.9|   74.0| 63.8| 
