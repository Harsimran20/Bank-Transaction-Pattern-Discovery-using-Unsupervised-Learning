# Bank Transaction Pattern Discovery using Unsupervised Learning

## Overview

This project demonstrates the use of **unsupervised machine learning** to discover patterns in bank transaction data. By applying **K-Means clustering** and **Principal Component Analysis (PCA)**, this analysis uncovers distinct groups within transaction data, providing insights into customer behavior and spending habits. 

The goal is to group customers into different clusters based on their transaction characteristics, such as transaction amount, merchant category, location, and time of transaction.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Steps](#steps)
- [Output](#output)
- [Cluster Insights](#cluster-insights)
- [License](#license)

## Dataset

The dataset used in this project is a CSV file named `bank_transaction_data.csv`, containing the following columns:

- **customer_id**: Unique identifier for the customer.
- **transaction_id**: Unique identifier for each transaction.
- **transaction_amount**: The amount spent or received in the transaction.
- **transaction_type**: Type of the transaction (e.g., debit, credit, ATM).
- **merchant_category**: The category of the merchant (e.g., groceries, fuel, entertainment).
- **transaction_date**: The date and time of the transaction.
- **location**: The location of the transaction.

Sample data:
```csv
customer_id,transaction_id,transaction_amount,transaction_type,merchant_category,transaction_date,location
1,1001,150,debit,groceries,2024-05-01 14:32:00,New York
2,1002,50,credit,fuel,2024-05-01 15:45:00,Los Angeles
3,1003,200,ATM,entertainment,2024-05-01 16:20:00,Chicago
...
## Installation
To run this project locally, ensure that you have Python 3.7 or higher installed. The following libraries are required:
pip install pandas matplotlib seaborn scikit-learn
Usage
Clone the repository to your local machine:
git clone https://github.com/your-username/bank-transaction-pattern-discovery.git
cd bank-transaction-pattern-discovery
Place the bank_transaction_data.csv dataset in the same directory as the script.

Run the script using the following command:

python bank_transaction_pattern_discovery.py
The script will perform the following steps:

Preprocess the data (encoding categorical features and extracting time-based features).

Standardize the features for clustering.

Apply PCA for dimensionality reduction.

Perform K-Means clustering to segment the transactions into clusters.

Visualize the clusters using a scatter plot.

Display a summary of the cluster characteristics (e.g., average transaction amount, most common merchant category).

## Steps
1. Data Preprocessing
Categorical features (transaction_type, merchant_category, location) are encoded using LabelEncoder.

The transaction_date column is parsed into a datetime format, and new features such as day_of_week and hour are extracted.

2. Feature Selection
The following features are selected for clustering:

transaction_amount

transaction_type_encoded

merchant_category_encoded

location_encoded

day_of_week

3. Standardization
The data is standardized using StandardScaler to normalize the feature values, ensuring that all features contribute equally to the clustering.

4. Dimensionality Reduction (PCA)
PCA (Principal Component Analysis) is applied to reduce the feature space to two dimensions, making it easier to visualize the clustering results.

5. Clustering (K-Means)
The K-Means clustering algorithm is applied to segment the dataset into 4 distinct clusters.

6. Visualization
A 2D scatter plot of the PCA components is generated, with each point representing a transaction, and different colors representing the different clusters.

7. Cluster Summary
The script outputs two summaries:

Average transaction amount per cluster.

Most common merchant category in each cluster.
