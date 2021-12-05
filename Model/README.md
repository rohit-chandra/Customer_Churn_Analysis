# Data Modeling

The Data Model is applied to the test Data to check if it’s accurate and houses all desirable features. As the data was highly imbalanced, we used Synthetic Minority Oversampling Technique(SMOTE), which involves duplicating samples in the minority class and Under Sampling Majority data set technique(UnderSampling), which randomly adds more minority observations by replication.

All our analysis is done with imbalanced data, SMOTE generated data and under-sampling generated data. While training models on these datasets, we performed hyper-parameter tuning using GridSearchCV, which loops over predefined hyper-parameters and fits the model to the training data using best parameter values obtained.
We considered following models to analyse the data:

- XGBoost
- Naive Bayes - GuassianNB, MultinomialNB, CompleteNB
- SVM
- Decision Trees


### 1. XGBoost Classifier
XGBoost is a decision-tree-based ensemble Machine Learning algorithm that uses a gradient boosting framework. The goal is to improve weak learners by using a gradient descent approach to minimise errors. When compared to other algorithms, it is thought to be exceptionally efficient and quick. 

### XGBoost classifier yields following graphs/results:

#### XGBClassifier (Imbalanced Data)-

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/Model/images/ROC_XGBClassifier.png)


#### XGBClassifier (Balanced Data - SMOTE)-

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/Model/images/ROC_XGBClassifierWithSMOTE.png)

#### XGBClassifier (Balanced Data - Under-sampling)-

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/Model/images/ROC_XGBClassifierUnderSampling.png)


#### XGBClassifier Results -

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/report/Images/xgbclassifier.png)



### 2. Naive Bayes Classifier 
The Bayes Theorem-based probabilistic machine learning method Naive Bayes(NB) is employed in a wide range of categorization problems.


### 2a). Gaussian Naive Bayes Classifier
It is a naive bayes algorithm that is unique. When the features have continuous values, it's employed particularly. It's also expected that all of the characteristics have a Gaussian distribution, or a normal distribution.

### Gaussian Naive Bayes Classifier yields following graphs/results:

#### Gaussian NB Classifier (Imbalanced Data)-

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/Model/images/ROC_GaussianNB_Classifier.png)

#### Gaussian NB Classifier (Balanced Data - SMOTE)-

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/Model/images/ROC_GaussianNB_Classifier_withSMOTE.png)

#### Gaussian NB Classifier (Balanced Data - Under-sampling)-

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/Model/images/ROC_GaussianNB_Classifier_withundersampling.png)

#### Gaussian NB Classifier Results -
![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/report/Images/GaussianNB.png)



### 2b). Complement Naive Bayes Classifier
It is well-suited to dealing with unbalanced data sets. Instead of calculating the probability of an item belonging to a certain class, we calculate the probability of the item belonging to all classes in complement Naive Bayes.

### Complement Naive Bayes Classifier yields following graphs/results:

#### Complement NB Classifier (Imbalanced Data)-

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/Model/images/ROC_ComplementNB_Classifier.png)

#### Complement NB Classifier (Balanced Data - SMOTE)-

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/Model/images/ROC_ComplementNB_Classifier_withSMOTE.png)

#### Complement NB Classifier (Balanced Data - Under-sampling)-

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/Model/images/ROC_ComplementNB_Classifier_withundersampling.png)

#### Complement NB Classifier Results -

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/report/Images/ComplementNB.png)



### 2c). Multinomial Naive Bayes Classifier
It is suitable for classification with discrete features (e.g., word counts for text classification). The multinomial distribution normally requires integer feature counts. 

### Multinomial Naive Bayes Classifier yields following results:

#### Multinomial NB Classifier (Imbalanced Data)-

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/Model/images/ROC_MultinomialNB_Classifier.png)

#### Multinomial NB Classifier (Balanced Data - SMOTE)-

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/Model/images/ROC_MultinominalNB_Classifier_withSMOTE.png)

#### Multinomial NB Classifier (Balanced Data - Under-sampling)-

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/Model/images/ROC_MultinominalNB_Classifier_withundersampling.png)

#### Multinomial NB Classifier Results -

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/report/Images/MultinomialNB.png)


### 3. Support Vector Classifier(SVC)
It is a linear model that can be used to solve classification and regression problems.It can solve both linear and nonlinear problems.The algorithm generates a line or hyper-plane that divides the data into categories. Support Vector Classifier yields following results:

### Support Vector Classifier(SVC) yields following graphs/results:

#### Support Vector Classifier(SVC) (Imbalanced Data)-

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/Model/images/ROC_SVM_Classifier.png)

####  Support Vector Classifier(SVC) (Balanced Data - SMOTE)-

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/Model/images/ROC_SVM_Classifier_withSMOTE.png)

####  Support Vector Classifier(SVC) (Balanced Data - Undersampling)-

![image](https://github.com/rohitchandra/Customer_Churn_Analysis/blob/main/Model/images/ROC_SVM_Classifier_withUnderSampling.png)

#### Support Vector Classifier(SVC) Results -

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/report/Images/svm.png)

### 4. Decision Tree 
It is supervised machine learning that categorises or predicts outcomes based on the answers to a previous set of questions. Decision Tree yields following results:

###  Decision Tree  yields following graphs/results:

#### Decision Tree (Imbalanced Data)-

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/Model/images/ROC_DT_Classifier.png)

####  Decision Tree (Balanced Data - SMOTE)-

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/Model/images/ROC_DT_Classifier_withSMOTE.png)

####  Decision Tree  (Balanced Data - Undersampling)-

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/Model/images/ROC_DT_Classifier_underSampling.png)

####  Decision Tree Results -

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/report/Images/decisionTree.png)

