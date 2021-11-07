# Fraud Detection using Binary Classification

### Abstract

The goal of this project to predict whether a transaction is a fraudulent one or not and thereby improve the efficacy of fraudulent transaction alerts for people and also help businesses reduce their fraud loss and increase their revenue.  

### Data

The [dataset](https://www.kaggle.com/c/ieee-fraud-detection/data) is provided by a payment service company, Vesta Corporation for a Kaggle competition. The dataset contains 189217 rows with 50 features. The data is highly imbalanced with about 3% fraud transactions.

*Features and Target Variables*

Target: Fraud or Valid
Features: Transaction amount, Debit vs. Credit, Product code, Timedelta and card information

### Algorithms

*Optimization Metrics*

When the positive class is smaller and the ability to detect positive sample correctly is our focus, Recall is the metric to optimize.

*Models* 

Logistic Regression, Random Forest and XGBoost were used before settling with XGBoost as the model with good scores on Recall while minimizing the False positive rate. 

Final XGBoost model after tuning hyperparameters using 5-fold cross validation has the Recall of 0.81 on the test set. 


### Tools

* Numpy & Pandas for data processing 
* Matplotlib and Seaborn for visualization
* Scikit-learn for modeling
* Random Oversampler

### Communication 
The slides and visuals are available in my [Github repository](https://github.com/pr-suresh/FraudDetection)


