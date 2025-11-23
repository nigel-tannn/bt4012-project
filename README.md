# BT4012 Fraud Analytics Project
Predicting Loan Application Fraud with Customer and Transaction Data

## Project Documents
- [Final Report](https://drive.google.com/file/d/1e_V5TycXFSNn8GwDfw5Jp45p3y6ZYzsx/view?usp=drive_link)
- [Presentation Slides](https://drive.google.com/file/d/1YR16xjixDURHP2pqSJ8ZbLJHTbvf7BdF/view?usp=sharing)

## Project Overview
This project implements various machine learning approaches to detect fraudulent behaviour in loan applications, enhanced with transaction-level behavioural data as supplementary signals. The goal is to classify each case as either legitimate or fraudulent using different models and compare their performance under class-imbalanced conditions.

# Models Implemented
- Logistic Regression
- Random Forest
- XGBoost

## Project Structure
```
├── data/
│   ├── loan_applications.csv     # Loan applications dataset
│   └── transactions.csv          # Transactions dataset
├── EDA.ipynb                     # Exploratory data analysis
├── model_training.ipynb          # End-to-end machine learning workflow
└── requirements.txt              # Project dependencies
```

## Data Preprocessing
The dataset consists of loan application records and customer transactions, each labeled as either legitimate or farudulent. The preprocessing steps include:
- Data cleaning
- Feature engineering
- Merging datasets
- Train-test split

## Model Training
Each model is hyperparameter-tuned to achieve optimal performance. The models are trained on the preprocessed loan applications data and engineered features derived from the transactions dataset.

## Dependencies
Required Python packages are listed in `requirements.txt`. Install them using:
```bash
pip install -r requirements.txt
```

## Performance Metrics
Models are evaluated using:
- Precision
- Recall
- F1-score
- ROC-AUC

## Future Improvements
- Use SMOTE or other resampling techniques to further address class imbalance