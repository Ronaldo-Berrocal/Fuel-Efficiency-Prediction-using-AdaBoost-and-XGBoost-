# Fuel-Efficiency-Prediction-using-AdaBoost-and-XGBoost-
This project compares models AdaBoost and XGBoost using Grid Search for predicting fuel efficiency (MPG) using the Auto MPG dataset from the UCI Machine Learning Repository. 
This project includes data preprocessing, exploratory data analysis (EDA), hyperparameter tuning using GridSearchSV, model evaluation using RMSE and $R^2$, parity plots and interpretation of feature importance. 

## Project Overview 

The efficiency optimization fuel in vehicles with intern combustion engines represent a fundamental problem in the automotive industry. Estimating vehicle fuel consumptions based on engine characteristics can support better vehicles desing and enviromental planning.

In this project, the algorithms supervised learning AdaBoost and XGBoost were implemented and compared to predict MGP values from the Auto MPG dataset. 

The machine learning framework includes:

- Data cleaning
- Handling missing values
- Feature preprocessing
- Exploratory Data Analysis (EDA)
- Hyperparameter optimization
- Model training
- Performance evaluation
- Model comparison 

## Dataset 

**Dataset:** Auto MPG Dataset 

**Source:** 
UCI Machine Learning Repository 

**Number of observations:**
398 vehicles 

**Target variable:** 
- MPG (Miles Per Gallon)

**Features include:**
- Cylinders
- Displacement
- Horsepower
- Weight
- Acceleration
- Model year
- Origin

## Objetives 

The main objetives of this project are: 

- Predict vehicle fuel efficiency. 
- Compare learnign supervised models: AdaBoost and XGBoost regressors.
- Optimize hyperparameters using GridSearchCV.
- Evaluate model performance using regression metrics.
- Identify the most influencial vehicle characteristics.

## Methodology 

The project follows the standard Machine Learning workflow:

1.- Data Loading: Dataset was loaded usign the repository UCI Machine Learning through official library *ucimlrepo*. 

2.- Data cleaning: Missing values in the variable dataset were imputed using the median.

3.- Exprolatory Data Analysis. 

4.- Data preprocessing: The values used during model training were not scaled because tree-based models do not require variable normalization. 

5.- Train-Test split: The dataset was split into $80\%$ for training (318 observations) and $20\%$ for testing (80 observations). The *random_state* parameter was set to $42$ for ensure reproducibility. 

6.- Hyperparameter tuning using GridSearchCV. 

7.- Model training.

8.- Model evaluation: The metrics reported was RMSE, $R^2$ and MAE. 

9.- Model comparison.









