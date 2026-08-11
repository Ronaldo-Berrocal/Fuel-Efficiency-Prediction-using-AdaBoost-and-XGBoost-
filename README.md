# Fuel-Efficiency-Prediction-using-AdaBoost-and-XGBoost-
This project compares models AdaBoost and XGBoost using Grid Search for predicting fuel efficiency (MPG) using the Auto MPG dataset from the UCI Machine Learning Repository. 
This project includes data preprocessing, exploratory data analysis (EDA), hyperparameter tuning using GridSearchSV, model evaluation using MAE, RMSE and $R^2$, parity plots and interpretation of feature importance. 

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

| Variable | Type | Description |
| :---: | :---: | :--- |
| `mpg` | Continuous | **TARGET** — Miles per gallon |
| `cylinders` | Integer | Number of cylinders (3–8) |
| `displacement` | Continuous | Engine displacement (in<sup>3</sup>) |
| `horsepower` | Continuous | Power (horsepower) |
| `weight` | Continuous | Vehicle weight (lbs) |
| `acceleration` | Continuous | 0–60 mph time (seconds) |
| `model_year` | Integer | Model year (70–82) |
| `origin_2` | Dummy | European origin (1=yes) |
| `origin_3` | Dummy | Japanese origin (1=yes) |

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

## Results 

**Model Performance — MPG Prediction**  
Evaluation metrics across baseline and hyperparameter-tuned (GS) models

| Model | RMSE | MAE | R<sup>2</sup> |
| :--- | :---: | :---: | :---: |
| `AdaBoost` | 2.4218 | 1.6681 | 0.8909 |
| `XGBoost` | 2.2973 | 1.7551 | 0.9018 |
| `AdaBoost (GS)` | 2.2467 | 1.6681 | 0.9061 |
| `XGBoost (GS)` | 2.3529 | 1.7754 | 0.8970 |


## Repository Structure

```text
Project-MPG-AdaBoost-XGBoost/    
├── data/                        
│    ├── auto_mpg_clean.csv         # clean dataset (398 cars, not NA)
│    ├── train_raw.csv              # 318 cars - unscaled training 
│    ├── test_raw.csv               # 80 cars - unscaled test 
│    ├── metrics_boosting.csv       # AdaBoost and XGBoost metrics
├── notebooks/
│    ├── EDA_preprocessing.ipynb
│    ├── XGBoost_AdaBoost.ipynb
├── figures/
├──
├── src/
├── README.md 
└── requirements.txt
```
## Reproducibility 

```text
pip install -r requirements.txt
```
Ejecute the notebooks (EDA → XGB/ADA). 

The EDA notebook generates files in /data/ for XGB and ADA.

All notebooks use `random_state=42` and same split an 80/20.


## Tecnologies 

- Python
- Pandas
- Numpy
- Scikit-learn
- XGBoost Regressor (baseline model and optimize with GridSearchCV optimization)
- AdaBoost Regressor (baseline model and optimize with GridSearchCV optimization)
- Matplotlib
- Seaborn 

## Contact 

Ronaldo Berrocal Reyes 

Berrocal-Reyes30@ciencias.unam.mx 

linkedin: www.linkedin.com/in/ronaldo-berrocal-reyes

Physicist & Data Scientist - UNAM 





