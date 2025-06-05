# Customer Churn Analysis and Predictive Modeling

A customer churn prediction model for predicting the churn probability of a hypothetical utility company named **Powerco**.

## Overview

The following project uses random forest classifier along with hyperparameter tuning for predicting customer churn. In addition, threshold tuning is performed to improve upon the recall metric
which proves needful to reduce the false negatives. A comprehensive exploratory data analysis and feature engineering is performed to optimize data representation for building a robust model.

## Project Structure

- **`Datasets/`**: The folder contains the relevant datasets related to the project. `client_data.csv` and `price_data.csv` are the original raw, unprocessed datasets used for EDA. Following EDA, `clean_data_after_eda.csv`
file contains the cleaned data resulting from exploratory data analysis. `data_for_predictions.csv` is the csv file containing the dataset obtained after feature engineering and used for the final model building and
`out_of_sample_data_with_predictions.csv` file contains the final dataset with churn predictions and prediction probabilities. An additional file `Data description.pdf` contains the descriptive information about the fields of the input datasets.

- **`notebooks/`**: The notebooks folder consists of 3 jupyter notebooks related to the project. `EDA.ipynb` file contains code regarding the exploratory data analysis done on the `client_data_csv` and `price_data.csv`
datasets. `Feature_engineering.ipynb` notebooks contains the code written for performing feature engineering on the `cleaned_data_after_eda.csv` file. `Churn prediction model.ipynb` file contains the preprocessing,
model building, evaluation and tuning code which concludes the project.

- **`Key Visualizations`**: The folder contains visualizations discovered during the EDA, feature engineering, and model building processes.

## Insights derived from analysis and model building

-  9.7% of the total companies churned where the major churners lie in the low consumption group i.e. companies consuming within 200,000 units of energy are the ones with highest churn numbers amounting to be 1,322 out of the 1,419 churned consumers.
- 5 of the 8 sales channel had the churn rate > 5% with 12.1% being the highest churn rate per channel.
- The distribution of churn by consumption was highly right-skewed, with the majority of customers concentrated in the lower consumption range. Similar is the case with forecasted fields.
- The customers who have 'gas' in their contract showed lesser churn than customers who did not have gas in their contract. Similarly, customers with 5 or lesser purchased products showed more churn than customers purchasing more than 5 products. This clearly indicates, the higher number of products a customer buys, the lesser is the churning risk.


## Installation and setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/utkarshere/Customer-churn-modelling-project.git
   cd Customer-churn-modelling-project

2. **Create a virtual environment**
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate

3. **Install Dependencies**
    pip install -r requirements.txt

4. Load the datasets and run the notebook.
      




