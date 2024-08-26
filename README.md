# The MPox Epidemic presented by the:
![image](https://github.com/user-attachments/assets/ce382959-92b4-4fa9-a641-f2fda0a4916a)


## Overview

World Health Organization (WHO) Director has determined that the upsurge of mpox in the Democratic Republic of the Congo (DRC) and a growing number of countries in Africa constitutes a public health emergency of international concern. Our Team embarked upon the goal of using image classification to identify early on the MPox virus. 

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Data](#data)
4. [Installation](#installation)
5. [Methodology](#methodology)
6. [Results](#results)
7. [Team](#team)
8. [References](#references)
9. [Class Presentation](#class)

## Introduction

This project utilized a dataset consisting of four image classes: Monkeypox, Chickenpox, Measles, and other. The project encompasses ML techniques such as Convolutional Neural Network (CNN), TensorFlow, and scikit-learn
that were used for data sourcing, transformation, exploratory data analysis and model training.

## Features

- Identify with a high accuracy rate the MPox virus via images through CNN.
- Train and test the model through classification using tensorflow.
- Standardized images and labels through scikit-learn.
- Gradio Interface to test the image classification model.

## Data

The dataset used in this project was sourced from Kaggle and includes 770 images.

The dataset was divided into 4 folders/classifications:

- Chickenpox [0]
- Measles [1]
- MPox [2]
- Normal [3]

### Image of ChickenPox
![image](https://github.com/user-attachments/assets/f8b362a4-9421-44e3-ab6e-e32fba740845)


### Image of Measles
![image](https://github.com/user-attachments/assets/8ff36fc1-9eed-4188-9b48-fde9f1cffea4)

### Image of Mpox
![image](https://github.com/user-attachments/assets/fd9663eb-bb25-4bf4-a0b1-a3126c096fb8)

### Image Normal
![image](https://github.com/user-attachments/assets/422843aa-fa4c-4537-85f7-ec18b17d2623)

## Installation

To run this project locally, you'll need Python and additional libraries installed. Use the following command to install the required libraries:

```bash
pip install scikit-learn
pip install keras
pip install matplotlib
pip install Tensorflow
pip install os
pip install requests
pip install pandas
pip install numpy
pip install opencv-python
pip install seaborn
pip install pil
pip install gradio
```

## Methodology 

1. ***Exploratory Data Analysis***  
* Took images classifcations and created an RGB value 
* Calculated the averages of the RGB to display the distribution of the various image classifications.
 ![image](https://github.com/user-attachments/assets/6d10fa7b-6096-43e5-b5ec-75695300bb10)

  
2. ***Data Preparation***  
* Created a dataframe from image path list and classes as labels  
* Split the dataset into training and test sets
* Used a label encoder to convert the labels to numbers
* Created a function to convert images into RGB values

3. ***Model Development***
* Utilized Convolutional neural network (CNN) due to its ability to recognize patterns in images.
* Converted images into a pickle file format that can be easily stored and transmitted
* Split the data into training and test sets
* Converted the series of images into a Numpy array in order to feed the datasent into the model for training and inference.


4. ***Model Validation***
* Trained and tested the model with an accuracy score of 93% for trained data and 53% for testing data
* Plotted training & validation accuracy and loss
![image](https://github.com/user-attachments/assets/f67e7f8a-9a93-4b6b-8551-317f07d2bd4a)


5.  ***Model Implementation***
* Gradio User Interface link https://6ef55b8b3176e2a3a7.gradio.live
* User is able to upload an image and the model will provide a classification of Chicken Pox, Mpox, Measles or Normal
  ![image](https://github.com/user-attachments/assets/8bf34850-605a-45ac-92ff-1f6bfbdd6856)


6.  ***Key Takeaways***
* Testing alternative Models for better accuracy results
* Images can be used to identify diferrent types of Viral skin infections, however more training data is needed especially with darker skin tones as the model is biased due to the sample set.

## Team

- Elizabeth Arias
- Dawn Kim
- Chearine Pringle
- Nico Contreras
- Eric Alicea
- Daniel Gallardo
  
## References

- Kaggle.com: https://www.kaggle.com/datasets/sujaykapadnis/monkeypox-skin-images-dataset-msid/data
  
## Class Presentation
- [link to Powerpoint on Googlecolab](https://docs.google.com/presentation/d/1W_JQiCiDouNFOa--RUsmTu8Y6nX2NVHU/edit#slide=id.p1)
