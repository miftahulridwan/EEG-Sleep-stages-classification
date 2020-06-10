# EEG Sleep Stages Classification
This project is an assignment for Deep Learning course in Master of Science in Data Science and Society program, Tilburg University. In this project, we deploy deep learning models to classify sleep stages using EEG brain signal dataset. The dataset is provided by the teacher, and the result is uploaded to [Codalab](https://competitions.codalab.org/competitions/23473?secret_key=fb6c5cc3-104a-4129-b416-b5e5cf22e3da "Assignemnt - Deep Learning Course - Block 3 - Spring 2020") to obtain model's accuracy against unseen data. We work as a group. However, in this repository, I only uploaded models that I was specifically working on. The details of this assignment are provided in the [first](https://github.com/miftahulridwan/EEG-Sleep-stages-classification/blob/master/Assignment_DL.pdf) and [second](https://github.com/miftahulridwan/EEG-Sleep-stages-classification/blob/master/Codalab_DL.pdf) project descriptions.

## Table of Directory
1. [Report](https://github.com/miftahulridwan/EEG-Sleep-stages-classification/tree/master/Report)
2. [Script](https://github.com/miftahulridwan/EEG-Sleep-stages-classification/tree/master/Src)

## Project Summary
The aim of this project is to obtain highest accuracy for sleep stages classification using Deep Learning models. For this task, we developed several models. In this repository, we present 2 models: (1) 2D Convolutional, and (2) 2D Convolutional + LSTM. For this kind of data, our 2D Convolutional model yields the highest accuracy on validation set. Thus, we proceed with grid search to find the best hyperparameter settings.
<br>

In spite of high accuracy in training and validation set, the accuracy suffers when trying to predict the test set. The summary of our model and accuracy are as follows:

Model | Training Accuracy | Validation Accuracy | Codalab accuracy
---- | ---- | ---- | ----
2D Convolution | 92.7% | 85.7% | 64.9%
2D Convolution + LSTM | 83.1% | 80.7% | 65.6%


As we could observe, our model is well behave in training and validation set. Thus, we suspect the performance drop is due to the difference in the data distribution between training and test data.

## Environment and Library
We deploy our code in Google Collaboratory environment. The [code](https://github.com/miftahulridwan/EEG-Sleep-stages-classification/blob/master/Src/EEG%20signal%20classification.ipynb) is written in Python using several libraries, namely:
1. Pandas
2. Numpy
3. Scikit-learn
4. Keras
