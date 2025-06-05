# Predictive Modeling of Water Pump Functionality

This project aims to predict the functionality status of water pumps using machine learning. We classify water pumps into three categories: **functional**, **non-functional**, and **functional but needs repair**, using supervised learning models on real-world data. The project was completed as part of the DSCI 5240 course at the University of North Texas.

## 🎯 Project Objective

To forecast the operational status of water pumps in remote regions to help organizations and governments prioritize repair and maintenance. Machine learning models are trained on pump characteristics such as installation year, source type, distance to the nearest town, and water quality.

## 📊 Dataset

- **Source**: Real-world dataset from DrivenData
- **Target Variable**: `Functioning Status`
- **Key Features**: Installation Year, Water Source Type, Pump Type, Water Quality, Funder, Distance to Town, Population Served

## 🛠 Models Used

- **Logistic Regression**
- **Random Forest**
- **Gradient Boosting** (🏆 Best performing model)

## 📈 Results Summary

| Model               | Accuracy | F1-Score |
|--------------------|----------|----------|
| Logistic Regression| 54%      | 0.50     |
| Random Forest      | 53%      | 0.52     |
| Gradient Boosting  | **56%**  | **0.64** |

Gradient Boosting achieved the best balance between precision and recall.

## ⚙️ Technologies

- Python (Pandas, NumPy, Scikit-learn)
- Jupyter Notebook
- Matplotlib, Seaborn for visualizations


