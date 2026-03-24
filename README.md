# NETWORK-INTRUSION-DETECTION-ON-CIC-IDS-2017
Network Intrusion Detection System using Machine Learning & Deep Learning

Dataset: CICIDS2017

📌 Project Overview 

This project presents an end-to-end Network Intrusion Detection System (IDS) designed to identify and classify malicious network traffic in IoT and enterprise environments. Using the CICIDS2017 dataset, the system detects 15 traffic classes (1 benign + 14 attack types) through a combination of advanced feature selection, robust preprocessing, and comprehensive model evaluation.

The project focuses on real-world generalization, ensuring models trained on balanced data perform reliably on naturally imbalanced network traffic.

⚙️ Key Highlights

Hybrid Feature Selection Pipeline:
Applied a three-stage selection process — ANOVA F-Test → Pearson Correlation → ExtraTrees (embedded method) — reducing dimensionality to 12 highly discriminative features.

Model-Specific Preprocessing:
Implemented Yeo–Johnson transformation and Min-Max scaling selectively for linear and distance-based models to handle skewed distributions while preserving tree-based model performance.

Imbalance-Aware Training:
Used SMOTE only on the training set and evaluated models on the original imbalanced test data to reflect real-world network conditions.

Comprehensive Model Comparison:
Evaluated multiple ML and DL models including KNN, Random Forest, XGBoost, LightGBM, Logistic Regression, Linear & RBF SVM, and LSTM.

High Performance:
Achieved 99% test accuracy with KNN and strong macro-F1 scores, demonstrating excellent generalization without overfitting.

Deployment-Ready:
Built a Streamlit-based web application for real-time intrusion prediction, complete with preprocessing pipelines and probability visualization.

🧠 Models Implemented

Decision Tree

Random Forest

XGBoost

LightGBM

Logistic Regression

K-Nearest Neighbors (KNN)

Support Vector Machine (Linear & RBF)

LSTM (Deep Learning)

📊 Dataset

CICIDS2017 — A modern, labeled intrusion detection dataset developed by the Canadian Institute for Cybersecurity, containing realistic benign and attack traffic.

🚀 Deployment

The trained models and preprocessing pipelines are integrated into a Streamlit application, enabling:

Manual input of network flow features

Real-time attack classification

Confidence visualization using class probabilities

🏆 Key Takeaway

This project demonstrates that with careful feature engineering, adaptive preprocessing, and proper evaluation strategy, traditional ML models such as KNN can outperform more complex approaches in intrusion detection tasks.

📌 Tech Stack

Python · Scikit-learn · XGBoost · LightGBM · Imbalanced-learn (SMOTE) · Streamlit · Pandas · NumPy
