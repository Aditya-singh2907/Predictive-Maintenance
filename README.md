# 🛠 Predictive Maintenance System

A machine learning-powered solution designed to predict equipment failures before they happen. This tool helps industries and manufacturers reduce downtime, improve safety, and optimize maintenance schedules using real-world sensor data and advanced classification models.

---

## 🌍 About the Project

Unplanned machinery failures can lead to significant downtime, revenue loss, and even hazardous conditions in industrial settings. This project aims to solve this challenge by using machine learning to forecast potential equipment failures with high accuracy.

The goal is to provide a lightweight and effective system that can:
- Analyze historical sensor and operational data
- Predict the likelihood of specific failure types
- Assist engineers in making data-driven maintenance decisions
- Extend the life of critical machinery

This project is ideal for industrial applications, academic research, and smart factory implementations.

---

## 🌟 Features

- *Multi-Class Failure Prediction*  
  Classifies multiple failure types (e.g., Heat Dissipation, Tool Wear, Power Failure) with strong accuracy using CatBoost.

- *Balanced Dataset via SMOTE*  
  Handles class imbalance using the Synthetic Minority Over-sampling Technique for improved generalization.

- *Robust Evaluation Metrics*  
  Evaluated using Accuracy, F1-Score, MCC, and Confusion Matrix to ensure model reliability.

- *Model Deployment Ready*  
  Trained model and scaler are saved using joblib for easy integration into production environments.

---

## 🛠 Technical Details

### Machine Learning Model:

- *Algorithm*: CatBoost Classifier  
- *Training Dataset Size*: 10,000+ samples  
- *Important Features*:
  - Type  
  - Air Temperature  
  - Process Temperature  
  - Rotational Speed  
  - Torque  
  - Tool Wear  
### Performance:
  - Training Accuracy: 92%  
  - Testing Accuracy: 86.77%  
  - MCC: 0.9116 (train)
  - MCC: 0.8645 (test)

### Backend & Logic:

- Developed using *Jupyter Notebook* for model training and evaluation
- *joblib* used to save and load the model and scaler
- Real-time inference based on user-provided input

### Libraries & Dependencies:

- pandas==2.2.3  
- numpy==2.2.6  
- matplotlib==3.7.2  
- seaborn==0.12.2  
- scikit-learn==1.6.1  
- catboost==1.2.3  
- imbalanced-learn==0.10.1   
- joblib==1.3.2

---

## ⚙ How It Works

1. User inputs operational values like temperature, torque, speed, and tool wear.
2. The system processes the input using the trained CatBoost model and pre-fitted scaler.
3. The model predicts the likelihood and type of failure.
4. The prediction is displayed on the web app along with a class label (e.g., "No Failure", "Heat Dissipation Failure", etc.).

---

## 📜 License

This project is licensed under the *MIT License*. You are free to use, modify, and distribute it for personal or commercial purposes. See the LICENSE file for more information.

---

## ❤ Acknowledgements

- Kaggle and other open datasets for providing real-world predictive maintenance data  
- Open-source community for machine learning and visualization libraries  
