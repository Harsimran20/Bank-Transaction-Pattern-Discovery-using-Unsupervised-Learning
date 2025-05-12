# Bank Transaction Pattern Discovery

## Overview

This project leverages unsupervised machine learning techniques to uncover hidden patterns in bank transaction data. By applying K-Means clustering and Principal Component Analysis (PCA), we provide deep insights into customer spending behaviors and transaction characteristics.

## 🚀 Key Features

- **Unsupervised Learning Analysis**: Discover meaningful transaction clusters
- **Advanced Data Preprocessing**: Extract rich features from transaction data
- **Dimensionality Reduction**: Use PCA to visualize complex transaction patterns
- **K-Means Clustering**: Segment transactions into distinct groups

## 📊 Dataset Highlights

The project uses a comprehensive bank transaction dataset with the following key attributes:
- Customer ID
- Transaction Amount
- Transaction Type
- Merchant Category
- Transaction Date
- Transaction Location

## 🛠 Installation

### Prerequisites
- Python 3.7+
- pip package manager

### Required Libraries
```bash
pip install pandas matplotlib seaborn scikit-learn
```

### Setup
1. Clone the repository
```bash
git clone https://github.com/your-username/bank-transaction-pattern-discovery.git
cd bank-transaction-pattern-discovery
```

2. Install dependencies
```bash
pip install -r requirements.txt
```

## 🔍 Usage

Run the main script:
```bash
python bank_transaction_pattern_discovery.py
```

## 📈 Analysis Steps

1. **Data Preprocessing**
   - Encode categorical features
   - Extract time-based features
   - Standardize data

2. **Dimensionality Reduction**
   - Apply Principal Component Analysis (PCA)
   - Reduce feature space to 2 dimensions

3. **Clustering**
   - Utilize K-Means algorithm
   - Segment transactions into 4 distinct clusters

4. **Visualization**
   - Generate 2D scatter plot of transaction clusters
   - Provide cluster characteristics summary

## 🔬 Key Outputs

- Cluster visualization
- Average transaction amount per cluster
- Most common merchant categories in each cluster

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

**Disclaimer**: This project is for educational and analytical purposes. Always ensure compliance with data privacy regulations when working with financial data.

7. Cluster Summary
The script outputs two summaries:

Average transaction amount per cluster.

Most common merchant category in each cluster.
