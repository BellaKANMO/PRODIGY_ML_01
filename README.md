# PRODIGY_ML_01 

# This project was carried out as part of my internship at Prodigy InfoTech as a Machine Learning intern
## House Price Prediction using Linear Regression
### Project Overview

This project implements a Linear Regression model to predict house prices based on:
- Square footage
- Number of bedrooms
- Number of bathrooms

The work follows a structured data preprocessing and modeling approach using Python and scikit-learn, entirely within a Jupyter Notebook.

### Repository Structure
```
.
├── README.md
├── .gitattributes
└── linear_regression_house_prices/
    ├── lin_reg_price_pred.ipynb
    ├── data/
    │   ├── train.csv
    │   └── test.csv
    ├── data_description/
    │   └── data_description.txt

```


- ```lin_reg_price_pred.ipynb``` : Main notebook containing data cleaning, modeling, and evaluation
- ```data/``` : Training and testing datasets
- ```data_description/``` : Description of dataset features

### Objective

Implement a linear regression model to predict house prices based on square footage, number of bedrooms, and number of bathrooms.

### Methodology

The work was carried out in two main phases:

#### 1. Initial Data Cleaning and Modeling

- Removed rows containing NaN values to obtain a clean dataset
- Applied StandardScaler for feature normalization
- Trained a Linear Regression model on the clean data
This step ensured a reliable baseline model using high-quality data.

#### 2. Price Imputation and Final Training

- Used the Linear Regression model to predict missing house prices
- Treated:
    - Clean data → training set
    - Data with missing prices → test set
- Filled missing values with model predictions
- Concatenated both datasets to create a fully clean dataset
- Re-trained the model using the previous Pipeline combining:
  - Standard scaling
  - Linear regression

### Tools & Libraries Used

All libraries used are commonly available in Jupyter environments:
- pandas
- numpy
- matplotlib
- scikit-learn

No additional installation is required

### Model

- Algorithm: Linear Regression
- Preprocessing: StandardScaler
- Training strategy: Pipeline-based workflow

### How to Run

- Clone the repository
     ```bash
   git clone https://github.com/your-username/your-repo-name.git
- Open ```lin_reg_price_pred.ipynb``` using Jupyter Notebook or Jupyter Lab
- Run the cells sequentially

### Notes

- The project focuses on clarity, correctness, and clean workflow
- No external utilities or scripts are required
- All steps are fully reproducible within the notebook
