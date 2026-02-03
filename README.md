
# TradeOps Sentinel: Automated Reconciliation & Risk Engine

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Finance](https://img.shields.io/badge/Domain-Trading%20Services-green)
![Status](https://img.shields.io/badge/Status-Operational-success)

---

## 📖 Executive Summary
In high-volume trading environments, manual reconciliation is the leading cause of settlement failures and operational risk. **TradeOps Sentinel** is an automated Python engine designed to modernize the **Middle Office** workflow, specifically targeting the responsibilities of a **Trading Services Analyst**.

This project ingests raw transaction logs, applies a **Hybrid Risk Model** (Rule-Based + Unsupervised Machine Learning), and performs automated reconciliation against external bank ledgers to ensure 100% accuracy in trade processing.

---

## 🚀 Key Features
* **Automated Reconciliation:** Replaces manual "stare and compare" Excel workflows with a Python script that instantly identifies breaks between Internal vs. External ledgers.
* **AI Anomaly Detection:** Utilizes an **Isolation Forest** (Unsupervised Learning) model to detect "Fat Finger" trades and operational outliers that static rules often miss.
* **Regulatory Monitoring:** Automatically flags transactions over $1M (Large Trader Reporting) and negative balance errors to ensure compliance.
* **Executive Reporting:** Generates a daily "Morning Operations Dashboard" summarizing Value-at-Risk (VaR) and outstanding operational breaks for management.

---

## ⚙️ Technical Architecture

| Component | Tech Stack | Functionality |
| :--- | :--- | :--- |
| **Data Simulation** | `NumPy`, `Pandas` | Generates synthetic trade blotters (Payment, Cash Out, Transfer) mimicking SWIFT/FIX logs. |
| **Risk Engine** | `Scikit-Learn` | **Isolation Forest** algorithm to detect high-dimensional outliers in trade data. |
| **Reconciliation** | `Pandas Merge` | Implements Left-Anti Joins to identify unmatched records (Breaks) between systems. |
| **Visualization** | `Seaborn`, `Matplotlib` | Generates a 4-panel risk report for operational decision-making. |

---

## 📊 Sample Output: Morning Operations Dashboard

*The system generates this report daily to prioritize the analyst's workflow.*

<img width="1550" height="985" alt="dashborad jp" src="https://github.com/user-attachments/assets/f8c83e1e-6996-4e72-9cf2-8ab68b8c5b52" />

---

## 💻 How to Run Locally

**1. Clone the Repository**
```bash
git clone [https://github.com/YourUsername/TradeOps-Sentinel.git](https://github.com/YourUsername/TradeOps-Sentinel.git)
cd TradeOps-Sentinel
---

## 💻 How to Run Locally

**1. Clone the Repository**
```bash
git clone [https://github.com/YourUsername/TradeOps-Sentinel.git](https://github.com/YourUsername/TradeOps-Sentinel.git)
cd TradeOps-Sentinel
