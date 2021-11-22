# Customer Churn Analysis

Contributors of the project :
1) Aishwarya Paruchuri : https://github.com/aishwarya95698
2) Archita Chakraborty : https://github.com/Archita22ind
3) Manjushree Barike Rajanna : https://github.com/MANJUSHREEBR
4) Rohit Chandra : https://github.com/rohit-chandra


**Understanding customer churn**

![](/images/customer_churn.jpeg)

Companies usually have a greater focus on customer acquisition and keep retention as a secondary priority. However, it can cost five times more to attract a new customer than it does to retain an existing one. Increasing customer retention rates by 5% can increase profits by 25% to 95%, according to research done by Bain & Company.

Churn is a metric that shows customers who stop doing business with a company or a particular service, also known as customer attrition. By following this metric, what most businesses could do was try to understand the reason behind churn numbers and tackle those factors, with reactive action plans.

If a company is not capable to identify these signals and take actions prior to losing the customer, there is no turning back. The customer churn data is a valuable asset for meaningful insights and to train customer churn models. Learn from the past, and have strategic information at hand to improve future experiences using machine learning.


## Dataset used : 
https://archive.ics.uci.edu/ml/datasets/Iranian+Churn+Dataset?TB_iframe=true&width=370.8&height=658.8

**Description of the data:**
Data is about churning telecom customers based on the features
* Complaints
* Subscription Length
* Charge Amount
* Seconds of Use
* Frequency of use
* Frequency of SMS
* Distinct Called Numbers
* Tariff Plan
* Status
* Age
* Customer Value


## Description of the problem being solved/investigated.

Using different multi-classification algorithms that give accurate classifications of the dataset and employ the recognized pattern from the data to make the best decision about each existing customer in the dataset set.

Questions to Investigate:

Main factors that lead customers to the cancellation decision based on the following metrics
* Poor service quality
* Delay on customer support 
* tariff plan
* Frequency of the complaints
* Age group of the customers
* Usage frequency

Usually, there is no single reason, but a combination of events that somehow culminate in customer discontinuation.

## Potential methods applied on the data set:

**We'll follow the life cycle of the Data science project:**

1)  **Data preprocessing**
  * Handle null values
  * Handle outliers

2) **Univariate and Bivariate analysis**
  * Infer relations between the input features and the predictor variable

3) **Feature Engineering**
  * Deriving new columns from the exsiting columns
  * Scaling column values(Using MinMaxScalar() method)

4) **Handle Imbalanced Dataset**
   Sampling techniques such as
  * Undersampling majority class set
  * Synthetic Minority Over-sampling Technique (SMOTE)

5) **Feature Importance**
  * Based on **correlation** we choose the most important features in the entire dataset

6) **Feature Selection** 
  * We select the best features using SelectKBest feature Selection technique

7) Training different **multi-classification models** with **Hyperpameter tuning** using gridsearch() with and without sampled data
  * XGBoost
  * Naive Bayes - GuassianNB, MultinomialNB, CompleteNB
  * SVM
  * Decision Trees
8) **Performance Metrics**
  * Compute different performance meterics like Confusion Matrix, classification report(Precision, Recall, F1 score)

9) **Multicollinearity Problem**  
   * Check for highly correlated features and selectively discard one of them

10) Compare the performance metrics of different models and derive conclusions to abate the customer churn


## How to measure success?
Since it is a classification problem we will use the following performance metrics:-
  * Accuracy
  * Confusion Matrics
  * Precision
  * Recall
  * F1 score
  * Receiver operating characteristic(ROC) and Area under the curve(AUC)






