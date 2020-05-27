## Deep-Forest
Code for paper: Emotion Recognition from Multi-Channel EEG via Deep Forest. Juan Cheng, Meiyao Chen, Chang Li, Yu Liu, Rencheng Song, Aiping Liu, Xun Chen. IEEE Journal of Biomedical and Health Informatics, 2020. 
## About the paper
* Title: [Emotion Recognition from Multi-Channel EEG via Deep Forest](https://ieeexplore.ieee.org/document/9096541)
* Institution: Hefei University of Technology
* Published in: 2020 IEEE Journal of Biomedical and Health Informatics
* DOI: 10.1109/JBHI.2020.2995767
## Instructions
* Before running the code, please download the DEAP dataset, unzip it and place it into the right directory. The DEAP dataset can be found [here](http://www.eecs.qmul.ac.uk/mmv/datasets/deap/index.html). Each .mat data file contains the EEG signals and consponding labels of a subject. There are 2 arrays in the file: **data** and **labels**. The shape of **data** is (40, 40, 8064). The shape of **label** is (40,4). Each .pkl file contains a numpy.ndarray variable. It stores the pre_processed data with the shape of (segments, window_size, width, height), in this paper, it is (2400,128,9,9).
* Please run the deap_preprocess.py to Load the origin .mat data file and transform it into .pkl file.
* Using deap.py to train and test the model (10-fold cross-validation), result of each fold will be saved in a .xls file.
* The DREAMER dataset can be found [here](https://zenodo.org/record/546113/accessrequest).
## Requirements
+ Pyhton 3.5
+ scipy
+ numpy
+ pandas
+ pickle
+ sk-learn

If you have any questions, please contact cmy@mail.hfut.edu.cn
