# Introduction

This machine learning project aims to predict startup success, defined as acquisition by a larger company, using supervised learning. Given the high failure rate (90%) of startups and the rise of crowdfunding, this project seeks to offer computational risk assessment tools for investors.

The data, sourced from CrunchBase and uploaded to Kaggle, includes 54,294 datapoints and 39 columns, encompassing categorical, date/time, and numerical data. The 'status' column, indicating whether a startup is acquired, operating, or closed, serves as the target variable.

I hope that people will contribute to this repository with the goal of improving model performance and interpretability.

# Code Overview
`main.ipynb` contains EDA, feature engineering, machine learning pipeline for training and evaluating Logistic Regression, Random Forest, SVC, and K Nearest Neighbors models, and some baseline interpretability exploration. Models are trained on investments_VC.csv.

`main_xgb.ipynb` builds upon `main.ipynb` by joining on investors.csv to create additional features. This jupyter notebook then contains a machine learning pipeline for training and evaluating an XGBoost model. `main_xgb.ipynb` also contains plots for global and local feature importance in this model.

# Environment
You can recreate the python environment using the environment.yml conda environment file by running these two commands in the terminal:

`conda env create -n startup-predictor -f environment.yml`

`conda activate startup-predictor`

You should be able to run `src/main.ipynb` and `src/main_xgb.ipynb`

# Author
Thomas Styron ([thomas_styron@brown.edu](thomas_styron@brown.edu))

# License
This project is licensed under the GNU GPLv3 license.