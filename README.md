Bank Customer Segmentation using RFM Analysis

📘 Project Overview

This project performs a comprehensive customer segmentation analysis for a bank using the RFM (Recency, Frequency, Monetary) model. The goal is to analyze the transactional behavior of the bank's customers to identify distinct segments, understand their value, and derive actionable business strategies. This helps the bank optimize resource allocation, personalize services, and enhance customer retention in a competitive financial landscape.

🎯 Objectives

RFM Analysis: Segment customers based on their transactional behavior:

Recency (R): How recently did the customer transact?
Frequency (F): How often do they transact?
Monetary (M): How much money do they spend?
Pareto Analysis: Identify the key customers who contribute the most to the bank's transaction volume.
Customer Strategy: Develop targeted strategies for each customer segment to maximize profitability and customer engagement.

📁 Dataset

The analysis is performed on the bank_transactions.csv dataset, which contains 1,048,567 anonymized customer transactions with the following features:

TransactionID: Unique identifier for each transaction.
CustomerID: Unique identifier for each customer.
CustomerDOB: Customer's date of birth.
CustGender: Customer's gender (M, F).
CustLocation: Customer's city/location.
CustAccountBalance: The balance in the customer's account.
TransactionDate: The date of the transaction.
TransactionTime: The time of the transaction (dropped during cleaning).
TransactionAmount (INR): The transaction amount in Indian Rupees (₹).

🛠️ Methodology & Steps

1. Data Cleaning & Preprocessing

Handled missing values in CustomerDOB, CustGender, CustLocation, and CustAccountBalance.
Removed duplicate transactions.
Converted TransactionDate and CustomerDOB to datetime objects.
Engineered a new Age feature and corrected inconsistencies (e.g., negative ages, unrealistic values).
Standardized CustGender values ('M' to 'Male', 'F' to 'Female').

2. Exploratory Data Analysis (EDA)

Analyzed the distribution of customer demographics (Gender, Location).
Examined the distribution of TransactionAmount and CustAccountBalance.
Investigated transaction patterns and identified top customer locations.

3. RFM Analysis

Recency: Days since the last transaction for each customer.
Frequency: Total number of transactions per customer.
Monetary: Total transaction amount per customer.

4. Customer Segmentation

Customers are segmented into groups based on their RFM scores (e.g., High-Value, Loyal, At-Risk, Churned) to facilitate targeted marketing and service strategies.

📊 Key Insights

Gender Distribution: A significant majority of transactions are made by male customers.
Transaction Patterns: The distribution of transaction amounts varies between genders, with specific peaks at common payment values.
Customer Value: A small percentage of customers (following the Pareto Principle) are likely responsible for a large portion of the transaction volume.
Age Demographics: The customer base is primarily composed of young to middle-aged adults, with ages cleaned and normalized for analysis.

🚀 Technologies Used

Python
Libraries:

pandas - Data manipulation and analysis
numpy - Numerical operations
matplotlib - Data visualization
seaborn - Statistical data visualization
datetime - Date-time object manipulation


Results and Business Implications

The RFM segmentation allows the bank to:

Identify High-Value Customers: Target them with premium services and loyalty programs.
Re-engage At-Risk Customers: Develop win-back campaigns for customers with low recency scores.
Optimize Marketing Spend: Focus resources on the most profitable segments.
Personalize Customer Experience: Tailor product offerings and communication based on segment characteristics.

