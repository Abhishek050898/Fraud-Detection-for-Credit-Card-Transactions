# Fraud Detection in Credit Card Transactions

## Overview
This project aims to detect fraudulent credit card transactions using **unsupervised anomaly detection** techniques. It leverages **Isolation Forest** and **Local Outlier Factor (LOF)** to identify anomalies in transaction data without requiring labeled fraud cases. The model is designed to be scalable and effective for real-world fraud detection.

## Technologies Used
- **Programming Language:** Python
- **Libraries:** Scikit-Learn, Pandas, NumPy, Matplotlib, Seaborn
- **Machine Learning Models:** Isolation Forest, Local Outlier Factor (LOF)

## Dataset
- The dataset contains anonymized credit card transactions with features transformed using **PCA (V1-V28)**.
- It includes a `Class` column, where:
  - `0` represents legitimate transactions.
  - `1` represents fraudulent transactions.

## Methodology
### 1. Data Preprocessing
- Standardized transaction data for improved model performance.
- Addressed class imbalance by training the model only on normal transactions.

### 2. Anomaly Detection Models
- **Isolation Forest:** Identifies anomalies by isolating transactions in randomly created partitions.
- **Local Outlier Factor (LOF):** Measures local density deviations to detect anomalies.

### 3. Model Evaluation
- Used precision, recall, and anomaly detection metrics to assess performance.
- Visualized fraud patterns using Matplotlib and Seaborn.

## Results
- The model successfully detects fraudulent transactions without requiring labeled fraud cases.
- Can be applied in **real-time fraud detection** for financial institutions.

## How to Use
```bash
# Clone the repository
git clone https://github.com/yourusername/fraud-detection.git

# Install dependencies
pip install -r requirements.txt

# Run the script
python fraud_detection.py
```

## Future Improvements
- Implement real-time detection with a streaming pipeline.
- Fine-tune hyperparameters for better anomaly detection.

## Contributors
- **Abhishek Kumar** 

## License
This project is licensed under the MIT License.

