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
## Method

### Models
We mainly tried the total of three models in our study:  
1. GCN model  
2. GAT model  
3. GraphSAGE model  
### Data preprocessing
For the data preprocessing part, we tried three methods: 
1. Fast Fourier Transform (FFT),  
2. Discrete Wavelet Transform (DWT), and  
3. Principal Component Analysis (PCA) to preprocess the dataset.
### Edge formulation
After K GCN layers, each node’s information would be spread to their k-hop neighbors. But as K get larger, the model may suffer over-smoothing problem. Hence, in this project, we only use three GCN layers: 
1. K = 3,
2. K = 6, and
3. K = 10 in our models.
### Pooling

### Other methods

## Setup
1. You have to save the dataset on your Google Cloud (please do not change the filename) . [Download dataset](https://purl.stanford.edu/bq914sc3730/ "link")
2. Load "Project.ipynb" to your Google colab. it can generate multiple 

## Reference
Model: <https://colab.research.google.com/drive/16GBgwYR2ECiXVxA1BoLxYshKczNMeEAQ?usp=sharing>  
Training Process: <https://colab.research.google.com/github/ga642381/ML2021-Spring/blob/main/HW01/HW01.ipynb>  
Other references: 
[1] <https://colab.research.google.com/drive/1I8a0DfQ3fI7Njc62__mVXUlcAleUclnb?usp=sharing>  
[2]	I. Omerhodzic, S. Avdakovic, A. Nuhanovic, K. Dizdarevic. “Energy Distribution of EEG Signals: EEG Signal Wavelet-Neural Network Classifier.”
[3]	Pari Jahankhani, Vassilis Kodogiannis, Kenneth Revett. “EEG Signal Classification Using Wavelet Feature Extraction and Neural Networks.”  IEEE John Vincent Atanasoff 2006 International Symposium on Modern Computing. IEEE, 2006.
[4]	Demir, Andac, et al. “EEG-GNN: Graph neural networks for classification of electroencephalogram (EEG) signals.” 2021 43rd Annual International Conference of the IEEE Engineering in Medicine & Biology Society (EMBC). IEEE, 2021.
[5]	Mehmet Akin. “Comparison of Wavelet Transform and FFT Methods in the Analysis of EEG Signals.” Journal of Medical Systems.
[6]	Andac Demir, Toshiaki Koike-Akino, Ye Wang, Masaki Haruna, Deniz Erdogmus. “EEG-GNN: Graph Neural Networks for Classification of Electroencephalogram (EEG) Signals.”	
[7]	Thomas N. Kipf, Max Welling. “Semi-Supervised Classification with Graph Convolutional Networks.” ICLR, 2017.

