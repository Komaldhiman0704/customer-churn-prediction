# Customer Churn Prediction Using Machine Learning (Telco Dataset)

## Project Overview
This project predicts customer churn for a telecom company using machine learning models. The goal is to determine if a customer will leave the service based on their subscription details and usage patterns. The workflow includes data loading, exploratory data analysis (EDA), preprocessing (handling missing values, encoding categorical features, addressing class imbalance with SMOTE), model training using tree-based classifiers (Decision Tree, Random Forest, XGBoost), and model evaluation with cross-validation metrics.

## Dataset
The dataset used is the Telco Customer Churn dataset from Kaggle. It has 7,043 customer records and contains features such as account tenure, monthly charges, total charges, and whether the customer churned (Yes/No).

Key points about the data:
- `TotalCharges` had missing values represented as spaces, replaced with 0.0 then converted to float.
- The target column `Churn` is imbalanced and addressed using the SMOTE technique.
- The dataset contains a mix of categorical and numerical features.

## How to Run

### Option 1: Run in Google Colab
1. Open the notebook `notebooks/Customer_Churn_Telco.ipynb` in Google Colab.
2. Upload the Telco Customer Churn CSV dataset or mount your Google Drive with the dataset.
3. Run the notebook cells step-by-step following the analysis and modeling process.

### Option 2: Run Locally
1. Clone this repository.
2. Create a Python virtual environment and activate it:

python -m venv venv
source venv/bin/activate # Linux/Mac
venv\Scripts\activate # Windows

3. Install dependencies:
pip install -r requirements.txt
4. Run the training script:
python src/train_models.py --data_path data/Telco-Customer-Churn.csv

5. Models and evaluation reports will be saved in the `models/` and `reports/` directories.

## Results
- Cross-validated accuracy and other classification metrics are reported.
- Confusion matrix and feature importance plots demonstrate the model performance.
- Models used: Decision Tree, Random Forest, and XGBoost.

## Notes
- Data preprocessing includes converting `TotalCharges` to float after handling empty strings.
- SMOTE oversampling is used to mitigate the class imbalance in the `Churn` target.
- Tree-based models are chosen for robustness and no need for feature scaling.

## Acknowledgments
- Dataset from Kaggle: [Telco Customer Churn](https://www.kaggle.com/blastchar/telco-customer-churn)
- Tutorial and project guide inspired by Siddhardhan’s YouTube channel: [Customer Churn Prediction Using ML](https://www.youtube.com/watch?v=qNglJgNOb7A)

## License
This project is licensed under the MIT License.
