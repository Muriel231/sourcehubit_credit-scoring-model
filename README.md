# Credit Scoring Model - Internship Task Report

## Objective
Build a machine learning model to predict a person’s creditworthiness using historical financial data. The goal is to classify whether a client will default on their credit card payment next month.



##  Dataset
The dataset contains 30,001 records of credit card clients with features such as:

- `LIMIT_BAL`: Credit limit  
- `SEX`, `EDUCATION`, `MARRIAGE`, `AGE`: Demographic info  
- `PAY_0` to `PAY_6`: Payment status history  
- `BILL_AMT1` to `BILL_AMT6`: Bill statement amounts  
- `PAY_AMT1` to `PAY_AMT6`: Payment amounts  
- `default payment next month`: Target variable (0 = no default, 1 = default)



##  Data Preprocessing
- Loaded the data and assigned column names  
- Converted all features to numeric and dropped missing values  
- Split data into features (`X`) and target (`y`)  
- Applied train-test split (80% training, 20% testing)  
- Used `StandardScaler` for feature scaling (required for Logistic Regression)



##  Models Used
- **Logistic Regression**  
- **Random Forest Classifier**



## Evaluation Metrics
- **Accuracy**: Correct predictions out of total samples  
- **Precision**: How many predicted defaults were actual defaults  
- **Recall**: How many actual defaults were correctly predicted



##  Results

| Model               | Accuracy | Precision | Recall  |
|---------------------|----------|-----------|---------|
| Logistic Regression | 0.8100   | 0.6927    | 0.2369  |
| Random Forest       | 0.8160   | 0.6380    | 0.3679  |



##  Analysis
- Random Forest performed slightly better in both accuracy and recall  
- Logistic Regression had slightly better precision  
- Random Forest is more effective for identifying defaulters (better recall)



##  Conclusion
The task was successfully completed using Python, pandas, and scikit-learn.  
Both models were trained and evaluated. Random Forest showed better performance in catching defaulters, which is critical in credit risk assessment.  
Further improvements could include hyperparameter tuning and feature engineering.
