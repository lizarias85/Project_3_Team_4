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

- Identify with a high accuracy rate the MPox virus via images.
- Train and test the model through classification using tensorflow.
- Gradio Interface to test the image classification model

## Data

The dataset used in this project was sourced from Kaggle and includes 770 images.

The dataset was divided into 4 folders/classifications:

- Monkeypox
- Chickenpox
- Measles
- Other


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
* Calculated the averages of the RGB to display the distribution
*  ![image](https://github.com/user-attachments/assets/6d10fa7b-6096-43e5-b5ec-75695300bb10)

  
2. ***Data Preparation***  
* Created a dataframe with image path list and classes as labels  
* Split the dataset into training and test sets
* Used a label encoder to convert the labels to numbers

3. ***Model Selection***
* Convolutional neural network (CNN) due to its ability to recognize patterns in images


4. ***Model Validation***
* Trained and tested the model with an accuracy score of 93% for trained data and 53% for testing data


5.  ***Model Implementation***
* Gradio User Interface link
* User is able to upload an image and the model will provide a classification of Chicken Poz, Mpox, Measles or Normal


## Results

TBD

### Image of Mpox
![image](https://github.com/user-attachments/assets/fd9663eb-bb25-4bf4-a0b1-a3126c096fb8)


### Image of ChickenPox
![image](https://github.com/user-attachments/assets/f8b362a4-9421-44e3-ab6e-e32fba740845)


### Image of Measles
![image](https://github.com/user-attachments/assets/8ff36fc1-9eed-4188-9b48-fde9f1cffea4)


### Image Normal
![image](https://github.com/user-attachments/assets/422843aa-fa4c-4537-85f7-ec18b17d2623)


The key takeaway blah blah blah

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
- link to Powerpoint on Googlecolab
