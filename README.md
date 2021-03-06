## Predicting Credit card fraud

### Abstract

The goal of this project is to predict whether a transaction is a fraudulent one or not and thereby improve the efficacy of fraudulent transaction alerts for people and help businesses reduce their fraud loss and increase their revenue. 

### Data

The [dataset](https://www.kaggle.com/c/ieee-fraud-detection/data) is provided by a payment service company, Vesta Corporation for a Kaggle competition. The dataset contains 189217 rows with 50 features. The data is highly imbalanced with only about 3% fraud transactions.

*Features and Target Variables*

Target: Fraud or Valid
Features: Transaction amount, Debit vs. Credit, Product code, Timedelta and card information, Categorical features

### Algorithms

*Optimization Metrics*
Our main focus is to be able to predict as many fraudulent transactions as possible while minimizing the False positive Rate. I calculate the Threshold based on this premise by maximizing the difference between True Positive Rate and False Positive Rate

*Models* 
Logistic Regression, Random Forest and XGBoost were used before settling with XGBoost as the model with good scores on Recall while minimizing the False positive rate. 

Final XGBoost model after tuning hyperparameters using 5-fold cross validation has the Recall of 0.88 on the test set. 


### Tools

* Numpy & Pandas for data processing 
* Matplotlib and Seaborn for visualization
* Scikit-learn for modeling
* Random Oversampler

### Communication 
The slides and visuals are available in my [Github repository](https://github.com/pr-suresh/FraudDetection)
