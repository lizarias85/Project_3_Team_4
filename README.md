# The MPox Epidemic presented by the:
![image](https://github.com/user-attachments/assets/ce382959-92b4-4fa9-a641-f2fda0a4916a)


## Overview

World Health Organization (WHO) Director has determined that the upsurge of mpox in the Democratic Republic of the Congo (DRC) and a growing number of countries in Africa constitutes a public health emergency of international concern. Our Team embarked upon the goal of using image classication to identify early on the MPox virus. 

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Data](#data)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Model Training](#model-training)
7. [Evaluation](#evaluation)
8. [Results](#results)
9. [Team](#team)
10. [References](#references)

## Introduction

This project utilized a dataset consististing of four image classes: Monkeypox, Chickenpox, Measles, and other. The project encompasses ML techniques such as Pytorch Lightning CNN, TensorFlow, and scikit-learn
that were used for data sourcing, transformation, exploratory data analysis and model training.

## Features

- Identify with a high accuracy rate the MPox virus via images
- TBD
- TBD

## Data

The dataset used in this project was sourced from Kaggle and includes two CSV files: `wine_data_white.csv` and `wine_data_red.csv`. These were combined into a single file, `wine_data_both.csv`.

The dataset contains the following columns:

- `Index`
- `fixed acidity`
- `volatile acidity`
- `citric acid`
- `residual sugar`
- `chlorides`
- `free sulfur dioxide`
- `total sulfur dioxide`
- `density`
- `pH`
- `sulphates`
- `alcohol`
- `quality`
- `Wine` (Type of wine: Red or White)

## Installation

To run this project locally, you'll need Python and additional libraries installed. Use the following command to install the required libraries:

```bash
pip install pandas numpy scikit-learn imbalanced-learn matplotlib statsmodels
```

## Usage

1. **Clone the repository:**

```bash
git clone git@github.com:N8sGit/group_project_2.git
cd group_project_2
```

## Methodology 

2. ***Data Preparation***  
* Synthetic data generation to correct extreme imbalances between the minority class (n=5) and majority class (n=2836).  
* Binning to correct for extreme data imbalances (merging the minority classes at the ends of the distribution)
* Noise elimination: Uses IsolationForest model to detect and remove outliers. 
* Feature selection: Uses Lasso Regression, mean squared error calculation, and variance inflation factor to detect the most what features don’t contribute to or distort the model. 

3. ***Model Selection***
* Hyper-parameter tuning 
* RandomizedSearchCV to traverse a randomized subspace 
* Manual experimentation and trial and error to determine that RandomForestClassifier is the most reliably performing algorithm 

4. ***Model Validation***
* Cross Validation to confirm consistency of results across several randomized folds
* A/B testing against raw data to contrast with our changes 

5.  ***Model Interpretation***
* Feature Importance comparison and analysis  

## Results

The project involved extensive exploratory data analysis, including descriptive statistics, correlation heatmaps, box plots, histograms, violin plots, and p-value analysis (which did not provide significant results). Key steps included:

- Analyzing the 'Quality' variable for correlation and removing highly correlated variables (free sulfur dioxide and density).
- Reviewing the distribution of all variables and removing outliers for model training.

### Describe Chart
![Describe chart](images/describe_chart.png)

### Correlation Heatmap
![Correlation Heatmap](images/correlation_heatmap.png)

### Box Plot
![Box Plot](images/box_plot.png)

### Histogram Charts
![Histogram Chart](images/histogram_chart.png)

### Violinplots
![Violinplots](images/violion_plot.png)

The key takeaway is that alcohol is the best predictor for high-quality wine using a Random Forest Model. Detailed results and visualizations can be found in the `results/` directory.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Team

- Elizabeth Arias
- Dawn Kim
- Chearine Pringle
- Nico Contreras
- Eric Alicea
- Daniel Gallardo
  
## References

- Kaggle.com: https://www.kaggle.com/datasets/sujaykapadnis/monkeypox-skin-images-dataset-msid/data
  
## Class presentation
- link to Powerpoint on Googlecolab
