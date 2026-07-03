# 🛡️ Endpoint Log Anomaly Detection Bot

A Machine Learning-based Endpoint Security System that detects anomalous behavior from Windows Security Event Logs using **Isolation Forest**, **K-Means Clustering**, **Graph Analysis**, and a **Real-Time Monitoring Bot**.

---

## 📌 Overview

This project analyzes raw Windows Security Event Logs, extracts behavioral features, and applies unsupervised machine learning techniques to identify suspicious activities.

The system consists of:

- Log Parsing & Preprocessing
- Feature Engineering
- Risk Level Assignment using K-Means
- Anomaly Detection using Isolation Forest
- Graph-based IP Relationship Analysis
- Real-Time Detection Bot
- Streamlit Dashboard for Visualization

---

## 🚀 Features

- ✅ Parse raw Windows Security Event Logs (JSON)
- ✅ Clean and preprocess security data
- ✅ Feature engineering for behavioral analysis
- ✅ Detect anomalies using Isolation Forest
- ✅ Assign Low / Medium / High Risk using K-Means clustering
- ✅ Identify Top Suspicious Users and IP Addresses
- ✅ Graph Analysis using NetworkX
- ✅ Real-time endpoint monitoring with Watchdog
- ✅ Interactive Streamlit Dashboard
- ✅ Automatic Security Alerts

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- NetworkX
- Streamlit
- Watchdog
- Joblib
- Matplotlib
- Seaborn

---

## 📂 Project Structure

```
Endpoint-Log-Anomaly-Detection-Bot/
│
├── SecurityProject.ipynb          # Model training and analysis
├── SecurityAnalysisReport.docx    # Project report
├── dataset/                       # Windows Security Event Logs
├── models/                        # Saved ML models
├── bot.py                         # Real-time monitoring bot
├── dashboard.py                   # Streamlit dashboard
├── requirements.txt
└── README.md
```

---

## ⚙️ Machine Learning Pipeline

```
Raw Windows Logs
        │
        ▼
Log Parsing
        │
        ▼
Preprocessing
        │
        ▼
Feature Engineering
        │
        ▼
Standard Scaling
        │
        ▼
PCA
        │
 ┌──────┴─────────┐
 ▼                ▼
K-Means     Isolation Forest
 ▼                ▼
Risk Level    Anomaly Score
        │
        ▼
Security Alert
```

---

## 📊 Risk Classification

The project groups endpoint events into three clusters using **K-Means**.

| Cluster | Risk |
|----------|------|
| Cluster 0 | 🟢 Low |
| Cluster 1 | 🟡 Medium |
| Cluster 2 | 🔴 High |

---

## 🤖 Real-Time Detection

The bot continuously watches incoming Windows Security Logs.

For every new event it:

- Parses the log
- Extracts features
- Applies preprocessing
- Runs PCA
- Predicts anomaly score
- Assigns risk level
- Generates alerts for suspicious activities

---

## 🌐 Dashboard

The Streamlit dashboard provides:

- Total Processed Events
- High-Risk Alerts
- Unique Users
- Average Anomaly Score
- Recent Alerts
- User Activity Charts
- Anomaly Distribution
- Real-Time Monitoring

---

## 📈 Graph Analysis

Using **NetworkX**, the project builds an IP relationship graph to identify:

- Highly connected IPs
- Suspicious communication patterns
- Degree Centrality
- Top 10 Most Influential IP Addresses

---

## 🧠 Models Used

### Isolation Forest

Used to detect unusual endpoint behaviors without labeled data.

### K-Means Clustering

Groups similar endpoint activities into different risk categories.

### PCA

Reduces dimensionality while preserving important information.

---

## 📦 Installation

Clone the repository

```bash
git clone https://github.com/ismailhalawa-ctrl/Endpoint-Log-Anomaly-Detection-Bot.git
```

Move into the project

```bash
cd Endpoint-Log-Anomaly-Detection-Bot
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run

Train / Analyze

```bash
jupyter notebook Log Anomaly Detection Code.ipynb
```
---

## 📄 Report

The full implementation details, methodology, experiments, and analysis are available in:

**Log Anomaly Detection Report.pdf**

---

## 👨‍💻 Author

**Ismail Halawa**

GitHub:
https://github.com/ismailhalawa-ctrl

---
