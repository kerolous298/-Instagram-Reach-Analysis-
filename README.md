# -Instagram-Reach-Analysis-
## Overview

This project analyzes Instagram post performance and predicts the reach (impressions) of posts using a machine learning model. It leverages a dataset containing metrics such as likes, saves, comments, shares, profile visits, and follows to train a PassiveAggressiveRegressor model. The project is implemented in Python using a Jupyter Notebook and includes data exploration and predictive modeling.

## Features

Loads and processes Instagram performance data from a CSV file.
Trains a machine learning model (PassiveAggressiveRegressor) to predict post reach based on engagement metrics.
Allows users to input custom features (e.g., likes, saves) to predict the reach of a hypothetical Instagram post.
Utilizes popular Python libraries for data analysis and machine learning.

## Dataset

The project uses a CSV file named Instagram data.csv, which contains the following columns:
Impressions: Total reach of the post.
From Home, From Hashtags, From Explore, From Other: Sources of impressions.
Likes, Saves, Comments, Shares: Engagement metrics.
Profile Visits, Follows: User actions after viewing the post.
Caption, Hashtags: Textual data associated with the post.
Note: The dataset (Instagram data.csv) must be placed in the same directory as the notebook for the code to run successfully.

## Requirements

Python 3.x
Required libraries:
pandas
numpy
matplotlib
seaborn
plotly
wordcloud
scikit-learn

## instagram-reach-analysis/

│
├── Instagram_Reach_Analysis.ipynb  # Main Jupyter Notebook
├── Instagram data.csv             # Dataset (required)
├── README.md                      # This file
└── requirements.txt               # (Optional) List of dependencies

## Model Details

Algorithm: PassiveAggressiveRegressor from scikit-learn.
Features Used: Likes, Saves, Comments, Shares, Profile Visits, Follows.
Target Variable: Impressions.
Train-Test Split: 80% training, 20% testing (test_size=0.2, random_state=42).
Performance: The model achieves a score of approximately 0.79 on the test set (R² score)
