# Mutual-Fund-Risk-Prediction

![GitHub Repo stars](https://img.shields.io/github/stars/dataWithSwathy/Mutual-Fund-Risk-Prediction?style=social)

---

## Project Description
This project focuses on predicting the risk levels of mutual funds using a classification approach. By analyzing multiple financial features such as expense ratio, assets under management (AUM), and returns over 1, 3, and 5 years, the model classifies mutual funds into various risk categories. The aim is to assist investors and financial analysts in understanding and categorizing mutual fund risks based on historical data and statistical modeling.

---

## Dataset Information
- **Source:** Kaggle
- **Sample Size:** 15,600 records
- **Columns (13):**
  - Expense Ratio (%)
  - AUM (Cr)
  - 1Y Returns (%)
  - 3Y Returns (%)
  - 5Y Returns (%)
  - Min Investment (₹)
  - Risk Level (Target variable with classes: Low, Moderately Low, Moderate, Moderately High, High, Very High)
  - ... (other columns as per dataset)

---

## Objectives
- Clean and preprocess mutual fund dataset, including handling missing values and outliers.
- Perform exploratory data analysis (EDA) to understand feature distributions and correlations.
- Encode the categorical target variable (Risk Level) for classification tasks.
- Balance the dataset using SMOTE to handle class imbalance.
- Train multiple classification models and tune hyperparameters via GridSearchCV.
- Compare model performances based on accuracy and classification reports.
- Visualize model results including PCA and UMAP dimensionality reductions and ROC-AUC curves.
- Provide actionable insights for mutual fund risk assessment.

---

## Analysis Summary & Insights
- The dataset contained some missing values filled with median imputation.
- Outliers were identified and removed using the IQR method for key numerical features.
- Risk levels are imbalanced; SMOTE effectively balanced the classes before training.
- Features like Expense Ratio, AUM, and multi-year returns have strong correlation patterns with risk levels.
- PCA and UMAP visualizations showed meaningful separations between risk categories.
- Random Forest and XGBoost models delivered the highest accuracy (~85%+), outperforming other classifiers.
- ROC-AUC analysis confirmed strong class-wise prediction capability.

---

## Models Used (Classification)
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Decision Tree Classifier
- Random Forest Classifier
- Support Vector Machine (SVM)
- Gaussian Naive Bayes (optional)
- XGBoost Classifier (optional, if installed)

---

## How to Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/dataWithSwathy/Mutual-Fund-Risk-Prediction.git
   cd Mutual-Fund-Risk-Prediction
