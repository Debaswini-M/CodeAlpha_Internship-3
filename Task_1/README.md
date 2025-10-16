# 💳 Credit Score Classification & Modeling (CodeAlpha Internship - Task 1)

This repository contains the analysis and machine learning model development for classifying or predicting credit scores. 

## 🎯 Project Goal

The project's implementation directly addresses all requirements of the assigned task:

| Requirement | Status | Implementation Detail |
| :--- | :--- | :--- |
| **Objective:** Predict creditworthiness. | **Completed** | Models predict **Credit Risk** (Good/Bad) using the German Credit Data. |
| **Approach:** Use classification algorithms. | **Completed** | **Logistic Regression, Decision Tree, and Random Forest** classifiers were used. |
| **Metrics:** Assess using Precision, Recall, F1-Score, ROC-AUC. | **Completed** | Model performance is rigorously evaluated and compared using these exact metrics. |

## 💾 Dataset

The project utilizes the **German Credit Data** dataset from the **UCI Machine Learning Repository**, which is commonly accessed via Kaggle.

* **Source:** [German Credit Data (UCI ML Repository)](https://www.kaggle.com/datasets/uciml/german-credit)
* **Target Variable:** The classification target is the **Credit Risk** (Good or Bad).


### 📝 Columns Used in the Model

The following **10 features** were selected and used for training the classification models:

* `Age`
* `Sex`
* `Job`
* `Housing`
* `Saving accounts`
* `Checking account`
* `Credit amount`
* `Duration`
* `Purpose`
* **Target:** `Risk`

---

## 🛠️ Methodology & Models

The analysis follows a standard data science pipeline:

1.  **Exploratory Data Analysis (EDA):** Initial exploration of data distribution, missing values, and correlation between features.
2.  **Data Preprocessing:** Handling categorical variables (One-Hot Encoding or Label Encoding), normalization/scaling of numerical features.
3.  **Feature Selection/Engineering:** Identifying and preparing the most relevant features for the models.
4.  **Model Training & Evaluation:**
    * **Models Trained:** Logistic Regression, Decision Tree Classifier, Random Forest Classifier.
    * **Evaluation Metrics:** The models were evaluated using **Accuracy**, **F1-Score**, and **ROC AUC** (as demonstrated in the model comparison plot).

## 📈 Model Performance Summary

| Model | Accuracy | F1-Score | ROC AUC |
| :--- | :--- | :--- | :--- |
| **Random Forest** | 0.733 | 0.825 | 0.747 |
| **Decision Tree** | 0.693 | 0.785 | 0.622 |
| **Logistic Regression** | 0.687 | 0.760 | 0.751 |

*Note: The **Random Forest Classifier** was the best-performing model based on the F1-Score, demonstrating the best balance between precision and recall for this dataset.*

## ⚙️ Dependencies

To run the Jupyter Notebook (`credit_Score.ipynb`), you will need the following libraries installed in your Python environment:

* `python (>= 3.8)`
* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`
* `scikit-learn` (for models and metrics)

## 👩🏻‍💻Author
`Debaswini`
