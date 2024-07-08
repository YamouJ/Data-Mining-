## Data Mining Techniques for Customer Retention: A Churn Analysis
In an effort to understand and predict customer churn, I conducted an in-depth analysis of a telecommunications company's dataset. The dataset comprises various attributes such as customer demographics, account information, and service usage patterns. To extract meaningful insights, I employed diverse data mining techniques, including feature selection, data preprocessing, and machine learning model evaluation. By dividing the dataset into training and test sets, I assessed each model's performance using metrics such as accuracy, precision, recall, and F1 scores. This approach enabled me to identify the most effective model for predicting customer churn, ultimately aiming to enhance customer retention strategies.

### Table of Contents

1. - [Introduction](#data-mining-techniques-for-customer-retention:a-churn-analysis)
2. - [Project Overview](#project-overview)
3. - [Dataset Description](#dataset-description)
4. - [Steps](#steps)
   - [Data Cleaning](#data-cleaning)
   - [Specifying the Columns and Splitting the Dataset](#specifying-the-columns-and-splitting-the-dataset)
   - [Standardization](#standardization)
   - [5-Fold Cross Validation and Classification Reports](#5-fold-cross-validation-and-classification-reports)
5. - [Results and Findings](#results-and-findings)
   - [Bar Plot Depicting Feature Importance](#bar-plot-depicting-feature-importance)
   - [Model vs Weighted Avg Of Various Metrics](#model-vs-weighted-avg-of-various-metrics)
6. - [Conclusion](#conclusion)

## Project Overview 

### Dataset Description: 
My project focuses on analyzing customer churn in the telecommunications industry, utilizing data mining techniques in Python to uncover key patterns and predictors. By examining detailed customer data, including demographics, account information, and service usage, the project aims to identify the factors contributing to customer attrition. The analysis reveals critical insights, such as the impact of contract type and payment method on churn rates, and the role of service quality in customer retention. The project underscores the importance of targeted strategies to enhance customer loyalty and reduce churn in the competitive telecommunications sector.

### Steps 
#### Data Cleaning 
1. To begin the data cleaning process, I examined the data types of each column in the dataset using print(df.dtypes) in Python Pandas. This step allowed me to understand the initial structure of the data and identify any potential mismatches between expected and actual data types, ensuring consistency and accuracy throughout the analysis.

<img width="500" alt="Screenshot 2024-07-05 at 4 47 13 PM" src="https://github.com/YamouJ/Data-Mining-/assets/167350506/6dce5972-4633-4358-afff-bf657082c2a8">

2. I examined the frequency of values in the "TotalCharges" column, removed empty entries, and converted the remaining data to floating-point format for consistency in analysis.
<img width="500" alt="Screenshot 2024-07-05 at 4 51 38 PM" src="https://github.com/YamouJ/Data-Mining-/assets/167350506/155a5c3b-9ff1-4755-9ffc-8c3a7646669f">

3. Randomly selecting a sample size of 1,869 from each class in the 'Churn' column effectively balances the dataset, ensuring unbiased representation across classes for further analysis.
<img width="750" alt="Screenshot 2024-07-08 at 2 07 26 PM" src="https://github.com/YamouJ/Data-Mining-/assets/167350506/35473624-f9fc-4640-a370-63240d80f71c">

5. The one-hot encoding creates binary columns for each category in the original categorical features, making them suitable for numerical analysis. The original categorical columns are then dropped, and I am left with a DataFrame containing only numerical features.
<img width="750" alt="Screenshot 2024-07-08 at 2 12 23 PM" src="https://github.com/YamouJ/Data-Mining-/assets/167350506/41944dc9-7e2d-4e2a-ac07-78b7f9c0c5b9">

6. #### Specifying the Columns and Splitting the Dataset
<img width="750" alt="Screenshot 2024-07-08 at 2 28 16 PM" src="https://github.com/YamouJ/Data-Mining-/assets/167350506/5ea73bcd-3852-4348-a572-84e67d551213">

7. #### Standardization
- Ensuring that features are on the same scale, which can improve the convergence of optimization algorithms and overall model performance.
<img width="750" alt="Screenshot 2024-07-08 at 4 27 53 PM" src="https://github.com/YamouJ/Data-Mining-/assets/167350506/d8d6a5a4-382f-4224-986d-a8e13ec04040">

9. PERFORMING 5-FOLD CROSS VALIDATION & CLASSIFICATION REPORTS
<img width="750" alt="Screenshot 2024-07-08 at 4 31 16 PM" src="https://github.com/YamouJ/Data-Mining-/assets/167350506/a518beb6-003f-45a6-beac-617d4f9508c9">

10. Bar Plot Depicting Feature Importance - Monthly Charges has the most importance while Phone Services has the least importance.
<img width="750" alt="Screenshot 2024-07-08 at 4 34 10 PM" src="https://github.com/YamouJ/Data-Mining-/assets/167350506/8b08e0a4-1bec-463b-8754-7a8e4081a773">

11. Model vs Weighted Avg Of Various Metrics
<img width="1095" alt="Screenshot 2024-07-08 at 4 38 33 PM" src="https://github.com/YamouJ/Data-Mining-/assets/167350506/9522ece0-30e0-4d6f-bece-e94487092d8d">


