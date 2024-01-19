# CipherCredit: Decoding Creditworthiness with Machine Learning

Credit scoring is becoming increasingly vital in financial decisions. Forbes reported an average credit card debt of $5,474 per borrower in Q3 2022, totaling $38 billion. The intersection of technology and finance, notably in credit evaluation, is rapidly evolving. This project aims to utilize machine learning to assess 'good' or 'bad' credit risks, offering insights into improving traditional financial models by utilizing the dataset found on Kaggle.

## Dataset

- Project dataset consists of application_record.csv and credit_record.csv, mergeable via
the client number (ID).
  a. application_record.csv includes personal/financial info (gender, car ownership, income,
etc.): 17 columns and ~440,000 rows
  b. credit_record.csv tracks monthly credit history, overdue days, and payments: 3 columns
and ~1,000,000 rows
- Found during research on credit scoring and finance machine learning on Kaggle.

## Data Preparation
-   De-duplication
-   Dealing with Sparse Columns
-   Handling Outliers
-   Imputing Missing Values using MICE
-   Balancing dataset using SMOTE

## ML Pipeline
<img width="724" alt="image" src="https://github.com/masadshoaib/Machine-Learning-for-Credit-Card-Application-Review/assets/56289860/8d5412d9-9736-4105-9907-ef3f8f74dbc7">

## Results
Random Forest performed the best after tuning hyperparameters. The results are shown below:
<img width="552" alt="image" src="https://github.com/masadshoaib/Machine-Learning-for-Credit-Card-Application-Review/assets/56289860/645884be-838d-4f2b-859e-af65d156682e">

Based on the feature importances of the variables, we recommend:
- Age and employment critical to approving credit card apps
- Have tailored strategies for different age groups and employment categories
- Consider personalized credit offerings based on family dynamics

