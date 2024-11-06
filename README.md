
# One-Class Anomaly Detection for Credit Card Fraud Detection

This project implements a one-class autoencoder-based anomaly detection system to identify fraudulent credit card transactions. By training solely on normal transactions, the model learns to detect anomalies, allowing for accurate fraud detection even in highly imbalanced datasets.

# Project Overview

Objective: Design a deep learning-based fraud detection system using one-class autoencoders to identify anomalies in credit card transactions.
Dataset: A credit card transaction dataset from Kaggle, containing 284,315 normal transactions and 492 fraudulent ones.

# Key Components

1. Model Architecture: A three-layer deep autoencoder trained on normal transactions to capture patterns specific to non-fraudulent activity.
2. Data Preprocessing:
   - Extracted normal transactions for training.
   - Standardized features to improve model accuracy.
3. Evaluation Metrics:
   - Confusion Matrix: Assesses classification performance.
   - Accuracy, Precision, Recall, F1 Score: Evaluates the balance between false positives and true positives.
4. Threshold Calculation:
   - DET (Detection Error Tradeoff) curve used to set an optimal threshold of 0.17 for anomaly detection.

# Results

1. Accuracy: 99.62%
2. Precision: 73.22%
3. Recall: 87.80%
4. F1 Score: 79.85%

The model demonstrated high accuracy and recall, indicating effective fraud detection with a trade-off in false positives.

# Strengths and Limitations

1. Strengths: 
  - High recall in identifying fraudulent transactions.
  - Adaptability to new fraud patterns with minimal labeled data.
2. Limitations: 
  - Relatively lower precision, resulting in a higher false positive rate.

# Future Enhancements

Advanced Techniques: Experiment with GANs or ensemble methods to improve precision.
Hybrid Models: Integrate the autoencoder with other anomaly detection algorithms.
Threshold Tuning: Further refine the threshold to balance false positives and negatives.


## Usage

1. Train the Model:
   Load `One_class_Anomaly_detection_using_autoencoders_for_fraud_credit_detection.ipynb` in Jupyter Notebook to train and evaluate the model.

-
