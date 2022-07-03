# Fraud Detection: Model Evaluation

In this notebook we will train several models and evaluate how effectively they predict instances of fraud using data based on [this dataset from Kaggle](https://www.kaggle.com/dalpozz/creditcardfraud).
 
Each row in `fraud_data.csv` corresponds to a credit card transaction. Features include confidential variables `V1` through `V28` as well as `Amount` which is the amount of the transaction. 
 
The target is stored in the `class` column, where a value of 1 corresponds to an instance of fraud and 0 corresponds to an instance of not fraud.

In the notebook we will go over the following sections:
- Load fraud detection data
- Instances of fraud
- Dummy Classifier 
- SVC Classifier: Precision Recall
- SVC Classifier: Confusion Matrix
- Logistic Regression: Precision Recall Curve
- Logistic Regression: Grid Search CV