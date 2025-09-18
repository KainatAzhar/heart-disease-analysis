# Predictive Analysis of Heart Disease

## 🎯 Project Goal

The primary goal of this project is to build a machine learning model to predict the presence of heart disease in a patient based on a set of medical attributes. This is a classic binary classification problem with significant real-world implications.

---

## 💾 Dataset

The dataset used is the **Heart Disease UCI** dataset, sourced from Kaggle. It contains 14 medical attributes, such as age, sex, chest pain type, and cholesterol levels, collected from multiple hospitals.

- **Link to Dataset:** [https://www.kaggle.com/datasets/redwankarimsony/heart-disease-data](https://www.kaggle.com/datasets/redwankarimsony/heart-disease-data)

---

## 📈 Project Workflow

The project followed a structured data science workflow:

1.  **Data Loading & Cleaning:** The dataset was loaded using the Kaggle API. A thorough cleaning process was performed to handle extensive missing values by either dropping columns with low completion rates or filling others with the median/mode.

2.  **Exploratory Data Analysis (EDA):** Visualizations were created to understand the distribution of key variables and the balance of the target variable (presence of heart disease).

3.  **Feature Engineering:** The multi-level target variable (`num`) was simplified into a binary outcome (`has_disease`). Categorical features like `sex` and `cp` were converted into a numerical format using one-hot encoding (`pd.get_dummies`) to make them machine-readable.

4.  **Model Training:** The preprocessed data was split into training (80%) and testing (20%) sets. A **Logistic Regression** model was chosen for its interpretability and solid performance as a baseline model.

5.  **Evaluation:** The trained model was evaluated on the unseen test set to measure its predictive performance.

---

## 📊 Results

The model achieved a strong and promising result for a baseline implementation:

- **Final Model Accuracy:** **80.43%**

The confusion matrix provided a deeper insight into the model's predictions:
- **True Positives (Correctly predicted sick):** 89
- **True Negatives (Correctly predicted healthy):** 59
- **False Positives (Incorrectly predicted sick):** 16
- **False Negatives (Incorrectly predicted healthy):** 20

Minimizing False Negatives would be the top priority for any future improvements to this model, given the critical nature of a medical diagnosis.

---

## 💻 Technologies Used

- **Python**
- **Pandas** (for data manipulation)
- **Matplotlib & Seaborn** (for data visualization)
- **Scikit-learn** (for model training and evaluation)
- **Jupyter Notebook / Google Colab** (for development)
- **GitHub** (for version control and portfolio)

---

## 🚀 How to Run

1.  Clone this repository to your local machine.
2.  Ensure you have Python and the necessary libraries installed (see `requirements.txt`).
3.  Place your `kaggle.json` API token in the root directory.
4.  Run the Jupyter Notebook `01-exploratory-data-analysis.ipynb`.
