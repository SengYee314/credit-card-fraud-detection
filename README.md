# Credit Card Fraud Detection

This project uses a credit card transaction dataset to explore, preprocess, and train machine learning models for fraud detection.

The main goal is to identify fraudulent transactions from highly imbalanced data, where normal transactions are much more common than fraud cases.

## Project Overview

- Loaded and explored the credit card transaction dataset
- Checked dataset shape, column information, and class distribution
- Split the data into training and testing sets
- Used SMOTE to handle class imbalance on the training data
- Trained Logistic Regression and XGBoost models
- Evaluated models using accuracy, precision, recall, classification report, and confusion matrix

## Best Model

The XGBoost model performed better than Logistic Regression.

Test results from the XGBoost model:

- Accuracy: 0.9991
- Precision: 0.6860
- Recall: 0.8468

Confusion matrix:

```text
[[56826    38]
 [   15    83]]
```

This means the model correctly detected 83 fraud cases and missed 15 fraud cases in the test set.

## Project Structure

```text
creditcard_fraud/
├── data/
│   └── raw/
├── notebooks/
│   ├── eda.ipynb
│   └── preprocess_train.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn
- XGBoost
- Jupyter Notebook

## Important Note

The dataset file is not included in this repository. The `data/raw/` folder is ignored because the CSV file may be large or sensitive.

To run this project, place the dataset here:

```text
data/raw/creditcard.csv
```

Then install the dependencies:

```bash
pip install -r requirements.txt
```
