# Predictive Modeling of Water Pump Functionality

This project applies supervised machine learning algorithms to predict the functionality status of water pumps. It was developed as part of the coursework for **DSCI 5240** at the University of North Texas under the instruction of **Javier Rubio Herrero**.

## 📌 Objective

To build predictive models that can classify water pumps into three functionality states:
- **Functional**
- **Non-functional**
- **Functional but needs repair**

Such classification helps organizations and governments optimize the allocation of resources for water infrastructure maintenance.

## 🧠 Problem Statement

Water is a critical resource, especially in remote regions. This project predicts pump status using features like:
- Installation year
- Distance to nearest town
- Water source type
- Population served
- Pump type
- Funding agency
- GPS coordinates

## 🗃 Dataset Overview

- Source: [DrivenData - Pump It Up](https://www.drivendata.org/competitions/7/pump-it-up-data-mining-the-water-table/)
- Rows: Each represents a water pump installation
- Target: `Functioning Status` (binary for modeling)

### Key Features:
- `water_source_type`
- `water_quality`
- `pump_type`
- `funder`, `payment_type`
- `installation_year`
- `population_served`
- `distance_to_nearest_town`

## 🔧 Data Preprocessing

- Missing values handled using mode or median
- Outlier detection via IQR
- Label Encoding for binary variables
- One-Hot Encoding for categorical variables
- MinMax Scaling for continuous variables
- Dropped `GPS coordinates` and `population_served` during modeling

## 🤖 Machine Learning Models

1. **Logistic Regression**
   - Training Accuracy: 54%
   - F1-Score: 0.50
   - Model struggled with recall for functional pumps

2. **Random Forest**
   - Training Accuracy: 100% (overfit)
   - Test Accuracy: 53%
   - F1-Score: 0.52

3. **Gradient Boosting Classifier** ✅
   - Training Accuracy: 66%
   - Test Accuracy: **56%**
   - F1-Score: **0.64**
   - Best performer across all evaluation metrics

## 📈 Evaluation Metrics

- Accuracy, Precision, Recall, F1-Score
- Confusion Matrix
- ROC and Precision-Recall Curves

## 📊 Key Insights

- **Pump Age**, **Distance to Town**, and **Water Source Type** are the most influential predictors.
- **Gradient Boosting** outperformed other models in precision, recall, and F1-score.
- Helps in prioritizing pump inspections and budget allocation.

## 🧠 Conclusion

Machine learning offers a powerful tool to predict equipment failure and support public infrastructure planning. This model aids in proactive maintenance of rural water pumps and promotes efficient water resource management.



