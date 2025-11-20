This project focuses on developing a machine learning pipeline to assess the creditworthiness of loan applicants. Using demographic and financial attributes, the system predicts whether an applicant is likely to be a good (1) or bad (0) credit risk.

The project demonstrates end-to-end data processing, feature engineering, class balancing, model training, evaluation, and insights relevant to real-world financial risk analysis.

Dataset Description:

The dataset used is a publicly available credit dataset containing a mix of numerical and categorical features. Key attributes include:

Loan duration

Loan amount

Applicant age

Job type

Gender

Housing type

Savings account status

Checking account balance

Loan purpose

Credit risk label: Good (1) or Bad (0)

Challenges Identified:

Missing values in categorical features

Class imbalance with fewer “Bad” credit cases

Mixed data types requiring tailored preprocessing

Importance of maximizing recall for the risky applicant group

Data Preprocessing Pipeline

The preprocessing workflow includes:

Missing Value Handling:

Imputation using "unknown" for categorical columns.

Encoding:

One-Hot Encoding for nominal features

Label Encoding for ordinal features

Scaling:

Standardization of numerical attributes using StandardScaler

Train-Test Split:

80% training, 20% testing

Class Balancing:

SMOTE applied on the training set to address minority class imbalance

Machine Learning Models:

The following models were trained and compared:

Random Forest Classifier
Achieved the best performance with over 85% accuracy and strong recall for the risky (Bad) class.

Gradient Boosting Classifier
Delivered balanced precision and recall.

AdaBoost Classifier
Effective for difficult cases but slightly less stable.

Logistic Regression
Used as a baseline; interpretable but lower performance.

Evaluation Metrics:

Models were evaluated using:

Accuracy

Precision

Recall

F1-Score

ROC-AUC

Confusion Matrix

The Random Forest model demonstrated the most robust performance across metrics, especially recall—critical in financial risk mitigation.
