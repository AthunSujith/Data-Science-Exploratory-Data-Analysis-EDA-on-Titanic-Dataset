# Titanic Survival Prediction 🚢🎯

This project analyzes and models survival outcomes from the Titanic disaster using machine learning. It is based on the Titanic dataset from Kaggle and includes data preprocessing, visualization, feature engineering, and classification modeling.

---

## 📁 Files Included

- `Titanic.ipynb` – Main Jupyter notebook for analysis and modeling
- `Titanic.csv` – Dataset used for the project
- `README.md` – Project description and usage guide

---

## 📊 Dataset Overview

The dataset contains demographic and passenger information for Titanic passengers:

| Column       | Description                         |
|--------------|-------------------------------------|
| PassengerId  | Unique ID for each passenger        |
| Survived     | Survival (0 = No, 1 = Yes)          |
| Pclass       | Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd) |
| Name         | Passenger name                      |
| Sex          | Gender                              |
| Age          | Age in years                        |
| SibSp        | # of siblings/spouses aboard        |
| Parch        | # of parents/children aboard        |
| Ticket       | Ticket number                       |
| Fare         | Passenger fare                      |
| Cabin        | Cabin number                        |
| Embarked     | Port of Embarkation (C, Q, S)       |

---

## 🧠 Features Created

- **Title Extraction**: Extracted titles (Mr, Miss, etc.) from the `Name` column.
- **FamilySize**: Combined `SibSp` + `Parch` + 1.
- **IsAlone**: Binary feature to indicate if passenger is alone.
- **FareBins & AgeBins**: Discretized versions of `Fare` and `Age`.

---

## 📈 Visualizations Used

- Correlation heatmap
- Fare vs. Survival scatter plot
- Survival rate by Pclass and Gender
- Age distributions
- Pie charts for gender survival

---

## 🔧 Machine Learning Models Used

- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)

Each model was evaluated using accuracy, confusion matrix, and cross-validation.
 Machine Learning Models Used

This project includes the implementation and evaluation of multiple machine learning classification algorithms to predict passenger survival on the Titanic.
✅ Models Implemented:

    Logistic Regression

        Simple and interpretable linear classifier.

        Suitable baseline for binary classification (Survived: 0 or 1).

    Decision Tree Classifier

        Tree-based model that splits features based on Gini impurity or entropy.

        Easy to visualize and explain.

    Random Forest Classifier

        Ensemble of decision trees using bagging.

        More robust and accurate than a single tree.

    Support Vector Machine (SVM)

        Finds the optimal hyperplane to separate classes.

        Works well in high-dimensional space.

    K-Nearest Neighbors (KNN)

        Non-parametric model that classifies based on nearest neighbors in feature space.

📈 Evaluation Metrics:

Each model was evaluated using:

    Accuracy Score

        Measures overall percentage of correct predictions.

    Confusion Matrix

        Provides TP, FP, TN, FN breakdown.

        Helps in visualizing errors (false positives/negatives).

    Cross-Validation

        Used 5-fold or 10-fold cross-validation to ensure model generalizability.

        Prevents overfitting by testing on different splits of the data.

| Model               | Accuracy | CV Score (Avg) |
| ------------------- | -------- | -------------- |
| Logistic Regression | 0.81     | 0.79           |
| Decision Tree       | 0.78     | 0.76           |
| Random Forest       | 0.83     | 0.81           |
| SVM                 | 0.80     | 0.78           |
| KNN                 | 0.77     | 0.75           |
