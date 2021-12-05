# Data Preprocessing

It’s a data mining approach for converting raw data into a
usable and efficient format.

Steps Involved in Data Preprocessing:
(A) Data Cleaning: There may be various useless and
missing elements in the raw data. Data cleaning is used to
deal with this aspect. It entails dealing with missing data
and noisy data.
Method used to find the null values: Missingno()

### 1. Checking for null values 

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/data_visualization/images/missing_values.png)

Techniques used to handle null values in the data:

#### i) Median: 

Some attributes, such as secondsOfUse and
customerValue, have outliers. We impute median value in
place of null values for these columns because mean is
prone to outliers.

#### ii) Mean : 

We impute mean values in place of null values for the remaining features that don’t have outliers.

#### (B) Outlier Detection:

Outliers are extreme values that deviate from other observations on data , they may indicate a variability in a measurement, experimental errors or a novelty. In other words, an outlier is an observation that diverges from an overall pattern on a sample.

#### Methods used to treat Outliers:

i) Drop the outliers
ii) Replace with median or a constant value

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/data_visualization/images/boxplot_afterCleaning.png)

### 2. Feature Scaling: 

This step is conducted to convert the data into a format that can be used in the mining process. Some of the classification models are based on probability, so we have scaled the data using MinMaxScalar() which transforms the values between 0 to 1 instead of StandardScalar() which transforms the data between -1 to 1.

### 3. Data Visualizations 

The graphical depiction of information and data is known as data visualisation. Data visualisation tools make it easy to examine and comprehend trends, outliers, and patterns in data by employing visual elements
like charts, graphs, and maps.

#### Distribution of all the categorical features:

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/data_visualization/images/Frequency_Distribution_afterCleaning.png)

####  Distribution of all the numerical features

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/data_visualization/images/frequency_distribution.png)

### 4. Feature Engineering

It involves deriving new features based on the existing features in the data set. In the data set, We have identified Age feature and performed feature engineering on it to create a new feature called AgeGroup to combine different age values in five different age intervals. The following table shows the age intervals:

![image](https://github.com/rohit-chandra/Customer_Churn_Analysis/blob/main/data_visualization/images/pie_chart_ageDistribution.png)

### 5. Correlation analysis


### 6. Feature Selection

We used SelectKBest feature selection technique to select top 13 features to train different multi-classification model. We can visualize with the help of horizontal bar plot shown below.