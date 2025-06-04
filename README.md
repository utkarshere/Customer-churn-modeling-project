# Customer Churn Analysis and Predictive Modeling

A customer churn prediction model for predicting the churn probability of a hypothetical utility company named **Powerco**.

## Overview

The following project uses random forest classifier along with hyperparameter tuning for predicting customer churn. In addition, threshold tuning is performed to improve upon the recall metric
which proves needful to reduce the false negatives. A comprehensive exploratory data analysis and feature engineering is performed to optimize data representation for building a robust model.

## Project Structure

- 'Datasets': The folder contains the relevant datasets related to the project. 'client_data.csv' and 'price_data.csv' are the original raw, unprocessed datasets used for EDA. Following EDA, 'clean_data_after_eda.csv'
file contains the cleaned data resulting from exploratory data analysis. 'data_for_predictions.csv' is the csv file containing the dataset obtained after feature engineering and used for the final model building and
'out_of_sample_data_with_predictions.csv' file contains the final dataset with churn predictions and prediction probabilities.

- 'notebooks': The notebooks folder consists of 3 jupyter notebooks related to the project. 'EDA.ipynb' file contains code regarding the exploratory data analysis done on the 'client_data_csv' and 'price_data.csv'
datasets. 'Feature_engineering.ipynb' notebooks contains the code written for performing feature engineering on the 'cleaned_data_after_eda.csv' file. 'Churn prediction model.ipynb' file contains the preprocessing,
model building, evaluation and tuning code which concludes the project.
