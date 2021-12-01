[![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://forthebadge.com)

# Customer Churn Analysis

## Contents

 * [Understanding customer churn](#understandin-customer-churn)
 * [Quick start](#quick-start)
 * [Folder Structure](#folder-structure)
 * [Installation](#installation)
 * [Steps to run the project](#steps-to-run-the-project)
 * [Dataset](#Dataset)
 * [Problem being investigated](#problem-being-investigated)
 * [Data Science Life cycle](#data-science-life-cycle)
 * [Conclusion](#Conclusion)
 * [Contributors](#Contributors)
 * [License](#License)



## Understanding customer churn

![](/images/customer_churn.jpeg)

Companies usually have a greater focus on customer acquisition and keep retention as a secondary priority. However, it can cost five times more to attract a new customer than it does to retain an existing one. Increasing customer retention rates by 5% can increase profits by 25% to 95%, according to research done by Bain & Company.

Churn is a metric that shows customers who stop doing business with a company or a particular service, also known as customer attrition. By following this metric, what most businesses could do was try to understand the reason behind churn numbers and tackle those factors, with reactive action plans.

If a company is not capable to identify these signals and take actions prior to losing the customer, there is no turning back. The customer churn data is a valuable asset for meaningful insights and to train customer churn models. Learn from the past, and have strategic information at hand to improve future experiences using machine learning.


## ⚡️ Quick start

### Folder Structure :

```shell
Customer_Churn_Analysis/
├── Model
│   ├── images   
│   ├── Model_building_with_clean_data.ipynb
│   └── README.md      
├── data
│   ├── Customer_churn_raw.csv
│   ├── Customer_churn_raw.csv
│   └── churn_final.csv
├── data_preprocessing
│   ├── CustomerChurnPrediction.ipynb
│   └── README.md
└── data_visualization   
│   ├── images
│   ├── Data visualization after cleaning.ipynb
│   ├── DataVisualization_BeforeDataCleaning.ipynb
│   ├── High_Level_Overview_of_dataset.ipynb
│   ├── sweet_report.html
│   └── README.md
└── images
│   ├── ...
│   └── customer_churn.jpeg
└── report
    ├── Images
    ├── Customer_Churn_Analysis.pdf
    ├── ieeeconf.cls
    └── main.tex    
```

### Installation :

Installation of below packages required before running the project

* `pip install anaconda-navigator`
* `pip install anaconda-navigator==2.1.1`
* `pip install analytics-python==1.4.0`
* `pip install certifi==2021.10.8`
* `pip install conda==4.10.3`
* `pip install conda-build==3.21.6`
* `pip install conda-verify==3.4.2`
* `pip install IPython==7.22.0`
* `pip install ipykernel==5.3.4`
* `pip install ipywidgets==7.6.5`
* `pip install jupyter_client==7.0.6`
* `pip install jupyter==1.0.0`
* `pip install Keras==2.3.1`
* `pip install missingno==0.4.2`
* `pip install pep8==1.7.1`
* `pip install plotly==5.3.0`
* `pip install pyforest==1.0.3`
* `pip install scikit-image==0.18.3`
* `pip install scikit-learn==1.0.1`
* `pip install seaborn==0.11.2`
* `pip install numpy==1.19.2`
* `pip install pandas==1.3.4`
* `pip install pandas-profiling==2.9.0`
* `pip install matplotlib==3.4.3`
* `pip install imbalanced-learn==0.8.1`
* `pip install nbclient==0.5.3`
* `pip install nbconvert==6.1.0`
* `pip install nbformat==5.1.3`
* `pip install notebook==6.4.6`
* `pip install nbdime==3.1.1`
   


### Steps to run the project :
```shell
 Clone repository here: https://github.com/rohit-chandra/Customer_Churn_Analysis.git
```

## Dataset

https://archive.ics.uci.edu/ml/datasets/Iranian+Churn+Dataset?TB_iframe=true&width=370.8&height=658.8

Data is about churning telecom customers based on the below features-

| Feature Name           |     Type       | Description                                   | 
| -----------------------|----------------| ----------------------------------------------|
| Call Failures          |  Categorical   | number of call failures.                      |
| Complains              |  Numerical     | binary (0: No complaint, 1: complaint)        |
| Call Failures          |  Categorical   | number of call failures                       |
| Subscription Length    |  Numerical     | total months of subscription                  |
|  Charge Amount         |  Categorical   | 0: lowest amount, 9: highest amount           |
| Seconds of Use         |  Numerical     | total seconds of calls                        |
| Frequency of use       |  Numerical     | total number of calls                         |
| Frequency of SMS       |  Numerical     | total number of text messages                 |
| Distinct Called Numbers|  Numerical     | total number of distinct phone calls          |
| Tariff Plan            |  Categorical   | binary (1: Pay as you go, 2: contractual)     |
| AgeGroup               |  Categorical   | 1: younger age, 5: older age                  |
| Status                 |  Categorical   | binary (1: active, 2: non-active)             |
| Customer Value         |  Numerical     | calculated value of customer                  |
| Churn                  |  Categorical   | binary (1: churn, 0: non-churn) - Class label |

       
## Problem being investigated

Using different multi-classification algorithms that give accurate classifications of the dataset and employ the recognized pattern from the data to make the best decision about each existing customer in the dataset set.

Questions to Investigate?

Main factors that lead customers to the cancellation decision based on the following metrics
* Poor service quality
* Delay on customer support 
* tariff plan
* Frequency of the complaints
* Age group of the customers
* Usage frequency

Usually, there is no single reason, but a combination of events that somehow culminate in customer discontinuation.

## Data Science Life cycle 


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


## Conclusion

Since it is a classification problem we will use the following performance metrics:-
  * Accuracy
  * Confusion Matrix
  * Precision
  * Recall
  * F1 score
  * Receiver operating characteristic(ROC) and Area under the curve(AUC)



### Contributors

* [Aishwarya Paruchuri](https://github.com/aishwarya95698)
* [Archita Chakraborty](https://github.com/Archita22ind)
* [Manjushree Barike Rajanna](https://github.com/MANJUSHREEBR)
* [Rohit Chandra](https://github.com/rohit-chandra)


##  License
