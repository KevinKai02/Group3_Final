# Group3_Final
## Topic
EEG Analysis with Graph Neural Network (GNN)
## Team Members
110062340 蔡皓宇 (Leader)  
110006267 張嘉俽  
110060019 周光祈  
110062226 王韋翔  
110062324 莊凱翔  
110062171 陳彥成
## Introduction
EEG measures and records the electrical impulses which is produced by the brain's neurons by attaching electrodes to the scalp. Convolutional neural networks (CNN) have been frequently used to extract subject-invariant features from EEG for classification tasks. However, traditional machine learning approaches such as CNN and RNN failed to utilize the spatial relations of the EEG electrodes. Therefore, we utilized graph neural network (GNN) to analyze EEG in this research. With GNN, we can exploit the spatial information, which shows potential for improvement.   
In this project, we tried several different data preprocessing methods, edge formulations, pooling methods, and models which have varying results and provide us more information about the nature of the models and EEG in general. And we tried to figure out that which combination would generate the best accuracy.

## Dataset 
Ten participants, aged 21 to 57 years (median age 30.5 years; 3 female; 1 left-handed), took part in the experiment. All participants reported normal color vision and either normal or corrected-to-normal vision.   
72 photographs of real objects were used as stimuli, taken from the 92-image set used in past RSA studies. The quantity of inanimate images is reduced in the set in order to ensure that each image category would contain the same number of exemplars—specifically, 12 images from each of the following six categories: Human Body (HB), Human Face (HF), Animal Body (AB), Animal Face (AF), Fruit Vegetable (FV), and Inanimate Object (IO).  
<img width = "404" height = "574" src = "https://github.com/KevinKai02/Group3_Final/blob/main/images/photograph_set.png">  
Each participant completed two experimental sessions, each containing three blocks, spaced between six and eight days apart. In total, each participant completed 72 trials of each of the 72 images, for a total of 5,184 trials per participant.

### [Download dataset](https://purl.stanford.edu/bq914sc3730/ "link")
## Method
## Setup
1. You have to save the dataset on your Google Cloud.  [Download dataset](https://purl.stanford.edu/bq914sc3730/ "link")
2. 
## Reference
Model: <https://colab.research.google.com/drive/16GBgwYR2ECiXVxA1BoLxYshKczNMeEAQ?usp=sharing>  
Training Process: <https://colab.research.google.com/github/ga642381/ML2021-Spring/blob/main/HW01/HW01.ipynb>  
Other useful reference: <https://colab.research.google.com/drive/1I8a0DfQ3fI7Njc62__mVXUlcAleUclnb?usp=sharing>  
