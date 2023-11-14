# **Credit Card Fraud Detection<a class="anchor"  id="top"></a>**
<center>
    <img src="https://www.xenonstack.com/hubfs/xenonstack-credit-card-fraud-detection.png" alt="Image" style="width:50%;height:50%;">
</center>


## Summary

#### Dataset:

The dataset presents an extensive collection of around 24.4 million credit card transactions, sourced from IBM's financial database. Capturing a wide spectrum of user interactions, the data provides a detailed snapshot of transaction behaviors, patterns, and potential vulnerabilities. 
Details include: **<span style="color:#007d79;"> User&card info, time&amount of transactions, merchant details, fraud detection flag</span>**.
Dataset Link - "https://www.kaggle.com/datasets/ealtman2019/credit-card-transactions/"

**Out of Total Transactions-**

**<span style="color:#007d79;">Non-Fraud-></span>**     24357143

**<span style="color:#007d79;">Fraud-></span>**       29757

**[Data Imbalancement](#di)**

As the Fraud transactions were much less than the valid transactions, the trained model would give the error as it does not have the adequate data to classify.so Random Under Sampling is used to bring a balance between data.


#### Project Highlight:

**[1. Data Overview](#data_overview)**

It will show the dataset's structure and distribution, inspecting its types of data and missing values that could impact the analysis.


**[2. Data Cleaning](#data_cleaning)**

Address inconsistencies and missing values to ensure the dataset's integrity, and remove redundancies to streamline the dataset, making it suitable for accurate and reliable analysis.
 
**[3. Exploratory Data Analysis](#eda)**

Examine patterns and trends of fraud transactions by visualizing fraud distribution on various metrics. From the EDA, we identified that certain variables significantly influence the fraud rate, and therefore, incorporated them into our predictive modeling:

* **[Transaction Amount:](#amount)**
Fraud is predominantly observed in transactions of smaller values.

* **[Geographical Distribution:](#geo)**
The distribution of fraud cases shows clear geographical differences.

* **[Time Variation:](#time)**
The distribution of fraud cases displays distinct time variations (By year, day of week, hour of day)

* **[Transaction Method:](#chip)**
Online transactions present the most significant vulnerability to fraud.


**[4. Fraud Detection with Machine Learning](#ml)**

* **[Data Preprocessing:](#data_preprocessing)**
Preprocessed the data to maintain consistency and balance, and then set up for further analysis.

* **[Model Optimization:](#randomforest)**
Used Random Forest model, made fine-tuning adjustments for better performance, and achieved a **<span style="color:#007d79;">78%</span>** success rate in correctly identifying fraud transactions.

**[5. Insights & Recommendations](#insights)**
* Through our analysis, we pinpointed three crucial variables influencing fraudulent activities: **<span style="color:#007d79;">the type of merchant (MCC), transaction amount, and the nature of the transaction (online vs. physical)</span>**. Recognizing these factors can guide financial institutions in refining their fraud prevention strategies.



**[ -Predicting the Fraud Transactions on User Input With the Model](#user)**
The User **<span style="color:#007d79;">Inputs the "csv" file</span>** and gets the **<span style="color:#007d79;"> predicted Output Classes</span>** 
