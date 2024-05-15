# Analysis_of_Customer_Churn
This repository contains my analysis on a dataset showing customer churn.

![image](https://github.com/ProfBesty/Analysis_of_Customer_Churn/assets/147350441/d9c9b0b3-da5c-495b-b611-deb1739de635)


## Problem statement
The financial services industry's ecosystem is dynamic and multidimensional, characterized by a complex interplay of factors that influence consumer behaviours. In this complex environment, the ability to retain customers is more than a strategic advantage; it is a requirement for long-term growth and sustainability. The inherent challenges of customer attrition for financial institutions include substantial revenue loss and the erosion of brand loyalty.

As a result, a Canadian bank facing challenges in retaining its customer base reached out to Datafied Technologies. The bank is experiencing customer churn, impacting overall customer satisfaction and revenue, as well as they lack insights into the factors influencing customer decisions to leave or stay with the bank. There is a need to identify and address factors contributing to customer churn proactively and to do that, they provided a churn database containing information on 10,000 bank customers over six months. 

## Overview of the Dataset
The dataset includes details on 10,000 bank customers spanning a period of six months. Each record in the dataset contains key information such as CustomerID, CreditScore, Geography, Gender, Tenure, Balance, and additional relevant attributes.

## Data Dictionary
- CustomerId: Each customer has a specific identification called a CustomerId.
- Surname: This serves as the client's last name. It is a categorical variable.
- Credit Score: This is the customer's credit score, which measures their creditworthiness numerically. Since a customer with a better credit score is less likely to quit the bank, a higher credit score often - - - implies a lower credit risk and can affect customer turnover.
- Geography: This feature indicates the country of residence of the customer.
- Gender: This feature represents the gender of the customer and can be either Male or Female.
- Age: The customer's age, in years.
- Tenure: The number of years that the consumer has been a bank client is shown by this characteristic.
- Balance: The balance shows how much money is in their bank account.
- NumOfProducts: This feature shows how many distinct banking products the client has with the bank. It accepts values between 1 and 4.
- HasCrCard: This variable indicates if the client has a credit card on file with the bank. The binary variable has the values 0 for "No" and 1 for "Yes."
- IsActiveMember: This feature indicates if the consumer is an active bank member. It's a binary variable once more, with 0 denoting "No" and 1 denoting "Yes."
- EstimatedSalary: This field contains data about the client's earnings.
- Churned: This variable tells us whether or not the consumer left (churned). The variable is binary, with 0 denoting "No" (the consumer stayed) and 1 denoting "Yes" (the customer left or "churned").

Data Source: Data Set (https://www.kaggle.com/code/kmalit/bank-customer-churn-prediction/data)

## Project Objective
The aim of this project is to provide a clear understanding of the bank's customer demographics, behaviours, and patterns of churn (customer attrition). The goal is to identify the key factors that influence customer churn, and then use these data-driven insights to develop strategic recommendations that can benefit the bank.

## Key Performance Indicators (KPIs)
We also defined metrics and KPIs that will help answer the business questions. Examples include:

- Total customers
- Churn ratio
- Retained customers

## Data Cleaning
The data cleaning process involves several steps, including:
- The values Yes and No in the HasCrCard column were replaced with "Has CrCard" and "No CrCard" respectively.
- The values Yes and No in the IsActiveMember column were replaced with "Active" and "Not Active" respectively.
- The values 1 and 0 in the Churned column were replaced with "Churned" and "Retained" respectively. A column titled Credit_Score_Group was created to group the credit score into; Poor (300 - 579); Fair (580 - 669); Good (670 - 739); Very Good (740 - 799) and Excellent (800 - 850).
- An Age_Group column was also created to group the ages into; Young Adult (20 - 39); Middle Adult (40 - 59) and Old Age (60+).
- A Credit_Score_Sort and Age_Group_Sort columns were created on power query to use in sorting Credit_Score_Group and Age_Group when visualizing.

## Dataset After Cleaning
![image](https://github.com/ProfBesty/Analysis_of_Customer_Churn/assets/147350441/17ccf6e7-8c2f-4dae-84de-4739979b3b84)

## Dashboard View
![image](https://github.com/ProfBesty/Analysis_of_Customer_Churn/assets/147350441/c0529e48-598e-45fd-a90e-cc78e585f854)

## Insight from Analysis
- The churn rate is approximately 20%.
- Spain had the lowest churn rate, while Germany and France had similar churn rates.
- Customers in the middle-aged group (40 to 59 years) have the highest churn number.
- Customers with a fair credit card score (between 580 and 669) have the highest churn rates.
- Customers who have only one distinct product with the bank have the highest churn rates, at 69.17%.
- Around 898 male customers and 1,139 female customers left (churned) the bank.

## Recommendations

- Focus on keeping middle-aged customers (40-59 years) as they have the most churn.
- Help customers with fair credit scores (580-669) improve their credit to reduce churn.
- Get customers to have more than one product, as those with just one product have the highest churn.
- Offer products that appeal to customers with low churn, like in Spain.
- Use models to find customers likely to churn and take action before they do.









