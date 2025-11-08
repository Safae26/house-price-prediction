# Boston Housing Price Prediction with XGBoost

## 📌 Project Overview
This project demonstrates a complete machine learning pipeline for predicting house prices in Boston using the XGBoost regression algorithm. The workflow covers data loading, preprocessing, exploratory data analysis, model training, and evaluation.

## Main Librairies : XGBoost, Scikit-learn, Pandas, NumPy, Matplotlib, Seaborn

## 🏠 Dataset Information
The Boston Housing Dataset contains real estate data from various suburbs in Boston, Massachusetts. The dataset includes 506 samples with 14 features:

| Feature | Description |
| :--- | :--- |
| **CRIM** | Per capita crime rate per town |
| **ZN** | Proportion of residential land zoned for lots over 25,000 sq.ft. |
| **INDUS** | Proportion of non-retail business acres per town |
| **CHAS** | Charles River dummy variable (1 if tract bounds river; 0 otherwise) |
| **NOX** | Nitric oxide concentration (parts per 10 million) |
| **RM** | Average number of rooms per dwelling |
| **AGE** | Proportion of owner-occupied units built before 1940 |
| **DIS** | Weighted distances to five Boston employment centers |
| **RAD** | Index of accessibility to radial highways |
| **TAX** | Full-value property tax rate per $10,000 |
| **PTRATIO** | Pupil-teacher ratio by town |
| **B** | 1000(Bk - 0.63)² where Bk is the proportion of black people by town |
| **LSTAT** | Percentage of lower status population |
| **price** | Median value of owner-occupied homes in $1000s (target variable) |

## 🛠️ Workflow

### 1. Data Loading
- Load the Boston house price dataset from a CSV file
- Dataset shape: 506 rows × 14 columns

### 2. Data Preprocessing
- Check for and handle missing values (none found in this dataset)
- Perform statistical analysis of the dataset

### 3. Exploratory Data Analysis (EDA)
- Analyze feature distributions
- Compute correlation matrix between features and target variable
- Visualize correlations using a heatmap
- Key observations:
  - **RM** (number of rooms) shows strong positive correlation with price (+0.70)
  - **LSTAT** (lower status population) shows strong negative correlation with price (-0.74)
  - **PTRATIO** (pupil-teacher ratio) shows moderate negative correlation (-0.51)

### 4. Model Training
- Split data into training and testing sets
- Use XGBoost Regressor for model training
- XGBoost is chosen for its scalability and high performance based on decision trees

### 5. Model Evaluation
- Assess model performance using appropriate regression metrics
- Evaluate on test set to measure predictive accuracy

## 📊 Key Insights
- The dataset is clean with no missing values
- Room count (RM) and socioeconomic status (LSTAT) are the strongest predictors of house prices
- XGBoost provides an effective solution for regression tasks with good performance

## 📈 Results
The XGBoost model effectively predicts Boston housing prices, leveraging the strong correlations identified in the EDA phase to make accurate predictions.
