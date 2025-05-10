# AI-Based-Insider-Threat-Detection
README.txt

Project Title: Insider Threat Detection System

Overview:
----------
This project aims to detect insider threats within an organization by analyzing user behavior using machine learning techniques. It utilizes logon, email, file, and device usage data to build models that can identify anomalous activities suggestive of malicious intent.

Key Features:
--------------
- Preprocessing of CERT v4.2 dataset including sessionization of user activity
- Feature engineering across multiple domains: logon, device, file, email
- Sequence modeling using Transformer-based Autoencoder
- Anomaly detection based on reconstruction error
- Evaluation using confusion matrix and threshold tuning based on True Positive Rate (TPR) and False Positive Rate (FPR)

Data Sources:
--------------
- CERT Insider Threat Dataset v4.2
- Processed CSVs: `logon_cleaned.csv`, `device.csv`, `file.csv`, `email.csv`
- Metadata: `LDPA` folder with user role and organizational hierarchy

Modeling Approaches:
---------------------
1. LSTM-CNN for logon behavior modeling
2. LSTM-Autoencoder for temporal anomaly detection
3. Transformer-based Autoencoder for multi-feature weekly behavior modeling
4. Individual models per data domain (logon, email, device)
5. SQLite database used to store per-user daily feature vectors


