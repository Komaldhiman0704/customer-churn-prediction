# Customer Churn Prediction with Machine Learning (Telco Dataset)

---

## 📋 Project Overview

This project implements a customer churn prediction system for a telecom company using machine learning techniques. The goal is to predict whether a customer will leave (churn) based on their account details and usage patterns.

The key steps followed in this project are:
- Data loading and initial inspection
- Exploratory Data Analysis (EDA) including visualization
- Data preprocessing (handling missing values, encoding categorical variables)
- Addressing class imbalance with SMOTE oversampling
- Model building using tree-based classifiers: Decision Tree, Random Forest, and XGBoost
- Model evaluation with cross-validation and metrics such as accuracy, confusion matrix, and classification report

---

## 📂 Dataset

The dataset used is the publicly available **Telco Customer Churn** dataset from Kaggle, containing 7,043 customer records with features like tenure, monthly charges, total charges, and churn status.

**Important notes about the dataset:**

- The `TotalCharges` column contains some missing values represented as spaces, replaced with 0.0, then converted to float.
- The target column `Churn` is imbalanced; addressed by SMOTE oversampling during training.
- Mix of categorical and numerical features are present.

---

## 🚀 How to Run

### Run in Google Colab (Recommended)

1. Open the notebook (`Customer_Churn_Telco.ipynb`) in [Google Colab](https://colab.research.google.com/).
2. Upload the Telco dataset CSV file or mount Google Drive containing it.
3. Run the notebook cells sequentially to reproduce the full workflow — from data analysis to model evaluation.

### Run Locally

1. Clone this repository:
git clone https://github.com/Komaldhiman0704/customer-churn-prediction.git
cd customer-churn-prediction



2. (Optional) Create and activate a virtual environment:
python -m venv venv
source venv/bin/activate # macOS/Linux
venv\Scripts\activate # Windows



3. Install required packages:
pip install -r requirements.txt


4. Open and run the notebook `Customer_Churn_Telco.ipynb` using Jupyter Notebook or JupyterLab.

---

## 📊 Results

- Multiple tree-based classifiers were trained and compared.
- Evaluated using cross-validation accuracy, confusion matrix, and classification reports.
- SMOTE effectively handled class imbalance, improving model performance.
- Visualizations include distribution plots and boxplots for EDA insights.

---

## 📝 Additional Information

- The notebook contains detailed comments and explanations aligned with the tutorial by Siddhardhan.
- The project focuses on practical machine learning workflow and model interpretability.
- Feel free to extend this project by adding hyperparameter tuning or alternative models.

---

## 🙏 Acknowledgments

- Dataset: [Telco Customer Churn - Kaggle](https://www.kaggle.com/blastchar/telco-customer-churn)
- Tutorial & Code Inspiration: [Siddhardhan's YouTube Video](https://www.youtube.com/watch?v=qNglJgNOb7A)

---

## 📄 License

This project is licensed under the MIT License.

---

Thank you for visiting! Feel free to ⭐ the repo if this was helpful.
