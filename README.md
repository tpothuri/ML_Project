# 🏡 House Price Prediction Using Machine Learning

This repository contains a comprehensive machine learning project that predicts housing prices in California using the **California Housing Dataset**. The project explores and compares various regression models to identify the most accurate methods for predicting real estate prices.

---

## 📌 Project Overview

## 🧠 Objective

To evaluate and compare the effectiveness of several machine learning regression techniques in predicting house prices and explore binary classification to determine whether a home’s price is above or below the median.

---

## 📊 Dataset

- **Source**: `fetch_california_housing()` from `scikit-learn`
- **Features**: 9 input features including median income, housing age, rooms, bedrooms, population, latitude, and longitude
- **Target**: Median house value

---

## ⚙️ Methodology

### 🔍 Data Preprocessing
- Loaded dataset with `pandas`
- No missing values found
- Features scaled using `StandardScaler`
- Dataset split into training and test sets (80/20)

### 🏗️ Models Used
- Random Forest Regressor
- XGBoost Regressor
- Gradient Boosting Regressor
- AdaBoost Regressor
- Decision Tree Regressor
- Support Vector Regressor (SVR)
- K-Nearest Neighbors (KNN)
- XGBoost Classifier (for binary classification)

### 📈 Evaluation Metrics
- R² Score
- Mean Absolute Error (MAE)
- Accuracy (for binary classification)
- ROC Curve & AUC

---

## 📉 Results

| Model               | R² (Train) | R² (Test) | MAE (Test) |
|--------------------|------------|-----------|-------------|
| Random Forest       | 0.97       | 0.81      | Low         |
| XGBoost             | 0.94       | 0.83      | Low         |
| Others              | Varies     | Lower     | Higher      |

- **Top Performers**: Random Forest & XGBoost
- **Binary Classification**: XGBoost Classifier performed well with a good ROC AUC

---

## 📊 Visualizations

- 📌 Correlation heatmap
- 📈 Actual vs. Predicted scatter plots 
- 📉 ROC curve for binary classification 

---

## 🛠️ Technologies Used

- Python
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost

---

## 🧩 Future Work

- Hyperparameter tuning
- Explore neural networks and deep learning models
- Incorporate more geographic and economic features


---

## 📁 Structure

```bash
.
├── house_price_prediction.ipynb  # Main Jupyter notebook
├── images/                  # Visualizations (scatter, heatmap, ROC)
└── README.md
