# Bank Transaction Pattern Discovery using Unsupervised Learning

This project uses unsupervised learning techniques (K-Means clustering and PCA) to discover patterns in bank transaction data.

## Installation

Ensure Python 3.7+ is installed and then install the required libraries:

```bash
pip install pandas matplotlib seaborn scikit-learn
Usage
Clone the repository:

bash
Copy
Edit
git clone https://github.com/your-username/bank-transaction-pattern-discovery.git
cd bank-transaction-pattern-discovery
Place the bank_transaction_data.csv dataset in the same directory as the script.

Run the script:
python bank_transaction_pattern_discovery.py
Steps
Preprocessing: Encodes categorical features and extracts time-based features.

Standardization: Scales features to ensure equal contribution to clustering.

PCA: Reduces feature space to 2 dimensions for visualization.

K-Means Clustering: Segments data into 4 clusters.

Visualization: Scatter plot of PCA components with clusters.

Cluster Summary: Displays average transaction amount and most common merchant category per cluster.

Results: Saves the clustered dataset as clustered_transactions.csv.

Output
Cluster Visualization: A scatter plot showing the clustering results.

Cluster Summary: Average transaction amounts and most common merchant categories per cluster.

Clustered Dataset: Saved to clustered_transactions.csv.

License
This project is licensed under the MIT License. See the LICENSE file for more details.
