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
* Age Group
* Tariff Plan
* Status
* Age
* Customer Value


## Description of the problem you’ll solve or the question you’ll investigate.

Using different classification algorithms that give accurate classifications of the dataset and employ the recognized pattern from the data to make the best decision about each existing customer in the dataset set.

Questions to Investigate:

Main factors that lead customers to the cancellation decision based on the following metrics
* Poor service quality
* Delay on customer support 
* tariff plan
* Frequency of the complaints
* Age group of the customers
* Usage frequency

Usually, there is no single reason, but a combination of events that somehow culminate in customer discontinuation.

## Potential methods you will consider apply (these can change as you play with the data).
We'll follow the life cycle of the Data science project:
1) Data preprocessing (handling null values/outliers)
2) Perform Univariate and Bivariate analysis to see the relation between the features and the predictor variable
3) Feature Engineering ( Deriving new columns from the exsiting columns, Scaling column values(standardization and normalization)
4) Feature Selection ( Methods: select K-best
5) Training the model
6) Performance Metrics

Also, since the target class is imbalanced we can use sampling techniques like methods like SMOTE: Synthetic Minority Oversampling Technique to handle the imbalanced dataset


## How to measure success?
Since it is a classification problem we will use the following performance metrics:-
* Confusion matrix
* precision
* recall
* F1 score






