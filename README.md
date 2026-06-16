# Transaction Anomaly & Fraud Detection Analysis

This project aims to build a machine learning model capable of performing fraud detection and anomaly identification based on financial transaction behavior. The analysis utilizes a dataset encompassing various transaction attributes, customer demographics, and usage patterns.

## Dataset Description

The dataset consists of thousands of transaction data samples. The key features analyzed include:
*   **Transaction Data:** `TransactionAmount`, `TransactionDate`, `TransactionDuration`, `TransactionType` (Credit/Debit), `Location`.
*   **Account & User Data:** `AccountBalance`, `PreviousTransactionDate`, `LoginAttempts`, `CustomerAge`, `CustomerOccupation`.
*   **Technical Context:** `Channel` (Online/ATM/Branch), `DeviceID`, `IP Address`, `MerchantID`.

## Workflow

The project was developed through several key stages:

1.  **Exploratory Data Analysis (EDA):** Descriptive statistical analysis and visualization to understand data distributions and correlations between features.
2.  **Data Preprocessing:** Applying *Feature Encoding* (such as *One Hot Encoding*) to handle categorical data.
3.  **Data Splitting:** Dividing the dataset into a *training set* and a *test set* while maintaining class proportions using the *stratify* parameter.
4.  **Classification Modeling:** Building and training a baseline model using the **Decision Tree** algorithm.
5.  **Advanced Algorithm Exploration:** Building a comparative model using ensemble algorithms such as the **Random Forest Classifier**.
6.  **Hyperparameter Tuning:** Optimizing model parameters using the grid search method to achieve the best performance.

## Visual Analysis Results (EDA)

This section presents the results from the Exploratory Data Analysis phase, providing insights into the dataset's characteristics prior to the modeling process.

### Correlation Matrix (Heatmap)
This visualization displays the level of linear correlation between numerical variables in the dataset.
![Correlation Matrix](images/Correlation%20Matrix.png)

### Feature Distribution (Histograms)
The following histograms illustrate the frequency distribution of key numerical features, helping to identify initial patterns or anomalies in the data.
![Feature Distribution](images/Feature%20Distribution.png)

## Model Evaluation Results

Model evaluation was conducted by comparing *Precision*, *Recall*, *F1-Score*, and *Accuracy* metrics on the *test set*. Below is a summary of the comparison:

| Evaluation Metric | Decision Tree (Base) | Random Forest (Tuned) |
| :--- | :---: | :---: |
| **Accuracy** | 0.95 | **0.99** |
| **Macro Avg F1-Score** | 0.95 | **0.99** |

Based on the test results, the **tuned Random Forest** model demonstrated significantly superior and more stable classification performance in detecting patterns within this dataset.