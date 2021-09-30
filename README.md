# Deep_learning_Image_Classification_Dog_Vision - Project Overview
This is my learning project when taking Machine Learning 0-Master course on Udemy. The goal of this project is to  to use deep learning for multil-class image classification using TrensorFlow Hub. The original project is from Kaggle.

## 1. Problem definition
dentify the breed of a dog giving an image of a dog.

When I am sitting at a cafe and take a piture of a dog, I want to know what breed of the dog it is.

## 2. Data
The data we are using is from Kaggle's dog breed identification competition

https://www.kaggle.com/c/dog-breed-identification/data

## 3. Code and Resource Used
Python version: 3.7
Packages:  pandas, numpy, matplotlib, sklearn, tensorflow, tensorflow_hub, IPython, os, datetime

## 4. EDA
I looked into the labels and the pictures in the data set, see if the numbers of labels (dog breed names) and pictures are matched with each other, or the number of picture of each label. I also checked if the picture is correctly labeled with the right breed name. 


![image](https://user-images.githubusercontent.com/70978272/135074867-507f9c41-739e-4d6c-93fc-4f48b3d468f4.png)
**the number of picture of each label**



![image](https://user-images.githubusercontent.com/70978272/135075292-c51a80cb-d914-4438-8ec9-ff32057b7491.png)

**tibetan_mastiff**


## 5. Data processing
Converting data into the form that is ready for training:

* Turning labels into arraies of boolean, then into integers.
* Split the data into training and validation data sets.
* Convert image into Numpy array, then into a Tensor
* Turning the data into batch (batch size 32), then create training and validation data batch.
* Visualize the data batch:

![image](https://user-images.githubusercontent.com/70978272/135140617-1e2dd57d-476a-4083-a2ea-560c512e3e67.png)


## 6. Modelling and evaluation

* Set up the input and ouput shapes (the images shape, in the form of Tensors) to the model
* Set up model URL from Tensors Hub: **Keras deep learning model** : https://www.tensorflow.org/guide/keras/sequential_model
* Create TensorBoard callback and early stopping callback
* First train the model with a subset of data as a test, to check and develope the fucntion to visualize our predictions and evaluate the model
* Train the moedel with the full data set, then make predictions on the test data.
* Make custom image predictions

![image](https://user-images.githubusercontent.com/70978272/135230918-47c8c04a-f452-4c53-8146-825fec59c92d.png)

