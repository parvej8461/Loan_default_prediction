# Loan Default Prediction

## Overview
This project aims to predict loan defaults by analyzing a dataset of loan applications and associated variables such as payment history, loan amounts, and underwriting data. The project utilizes machine learning algorithms to classify whether a loan will default or not based on the input features.

## Project Workflow
1. **Data Loading**: Three datasets (`loan.csv`, `payment.csv`, `clarity_underwriting_variables.csv`) were merged to create the final dataset for analysis.
2. **Data Preprocessing**: 
   - Missing values were handled using median imputation for numerical features and constant value imputation for categorical features.
   - Data was encoded using Label Encoding for categorical variables.
   - The dataset was scaled using StandardScaler for numerical features.
3. **Exploratory Data Analysis (EDA)**: Visualization and statistical summaries were performed to understand the relationships between features, including loan amounts, payment statuses, and fraud indicators.
4. **Feature Engineering**: 
   - New features were created by encoding categorical variables.
   - The target variable (`is_default`) was created, indicating whether a loan was defaulted or not based on loan status.
5. **Model Training**: 
   - Various machine learning models were trained and evaluated, including Logistic Regression, Decision Tree, and Random Forest classifiers.
   - The dataset was undersampled to handle class imbalance.
6. **Model Evaluation**: Classification reports and confusion matrices were used to evaluate model performance. The Random Forest model also provided insights into feature importance.

## Dependencies
- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn


## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/loan-default-prediction.git
   cd loan-default-prediction
   ```

2. Ensure you have the necessary CSV files (`loan.csv`, `payment.csv`, `clarity_underwriting_variables.csv`) . The files are private but similar datasets may be available in Kaggle.

3. Run the Jupyter notebook or Python scripts to execute the project.

## Results
- The Random Forest model provided the highest accuracy in predicting loan defaults. Key features that influenced the model included loan amount, payment frequency, and fraud indicators.

## Future Improvements
- Further tuning of the models could improve accuracy.
- Incorporating additional data sources could enhance the model’s robustness in real-world applications.
