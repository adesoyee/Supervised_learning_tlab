**Financial Fraud Dataset - Basic Pipeline**

NOTE: READ THIS DOCUMENT THOROUGHLY FOR SUCCESS

**Background**
In the realm of supervised learning algorithms, the challenge of extracting meaningful signals from noisy datasets is a recurring theme. This is particularly relevant when dealing with imbalanced datasets where the class of interest, such as fraud in financial transactions, is a minority. The Financial Fraud Dataset presents an opportunity to explore strategies for effectively identifying fraudulent transactions while minimizing false positives.

**Dataset Overview**
The synthetic dataset comprises both discrete and continuous variables, each providing insights into bank transactions. Key columns include:

Step: Timestamp of the transaction, representing hours in the dataset.
Type: Type of transaction.
Amount: Amount of money transferred.
NameOrig: Origin account name.
OldBalanceOrg: Origin account balance before the transaction.
NewBalanceOrg: Origin account balance after the transaction.
NameDest: Destination account name.
OldbalanceDest: Destination account balance before the transaction.
NewbalanceDest: Destination account balance after the transaction.
IsFlaggedFraud: A "naive" model flagging a transaction as fraudulent if it exceeds 200,000 (currency not USD).
IsFraud: Binary indicator of whether the transaction is fraudulent.

**Project Objectives**
This project involves creating a comprehensive machine learning pipeline following classic steps:

Initial EDA (Exploratory Data Analysis):
Perform univariate, bivariate, and multivariate exploratory analysis.
Create relevant graphs to formulate hypotheses.
Explore relationships among predictors and the target variable.
Data Cleaning, Wrangling & Pre-processing:
Clean and wrangle the dataset based on EDA insights.
Handle null values, remove unnecessary columns, eliminate outliers, and address incorrectly formatted data.
Save the pre-processed dataframe as a new CSV file for subsequent steps.
Model Creation, Hyperparameter Search, and Model Evaluation:
Implement a RandomForestClassifier or GradientBoostingClassifier.
Perform train-test splits.
Conduct hyperparameter tuning using GridSearchCV or RandomizedSearchCV.
Re-train the model with optimal hyperparameters and evaluate its performance using F1 score.

**Method Used**
Mathplotlib Python Numpy Seaborn Pandas Scipy Jupyter
**Technologies Used**
Data Visualization T-Tests/P-Value Inferential Statistics Gradient Boosting Classifier
**Report**
Answer the following questions in a separate document:
i. I hypothsized that there is no correlation between "isFraud" and "NewbalanceOrig" Null hypothsis: There is a correlation between shares and likes in a post. My hypothesis was proven correct. There was actually no correlation between most of the graphs. There was one that had a postive correlation and that was between oldbalanceOrg' and 'newbalanceOrig.' This might have been because when money leaves an account it decreases so theres that. 
ii. Criteria for dropping or keeping columns based on EDA was whether a column was necessary to interpret data.
v. Final F1 Score is 0.029413867899792622
