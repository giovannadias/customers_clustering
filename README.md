# Customer's Clustering 🛒

This project was made with the [Customer Personality Analysis](https://www.kaggle.com/imakash3011/customer-personality-analysis) database. 

## 💡 Problem Statement
Customer Personality Analysis is a detailed analysis of a company’s ideal customers. It helps a business to better understand its customers and makes it easier for them to modify products according to the specific needs, behaviors and concerns of different types of customers.

With this project, the store will have groups os similar customers, which will help create better marketing and sales strategies to increase revenue.

## 📚 Data Dictionary
Need to perform clustering to summarize customer segments.

- ID: Customer's unique identifier
- Year_Birth: Customer's birth year
- Education: Customer's education level
- Marital_Status: Customer's marital status
- Income: Customer's yearly household income
- Kidhome: Number of children in customer's household
- Teenhome: Number of teenagers in customer's household
- Dt_Customer: Date of customer's enrollment with the company
- Recency: Number of days since customer's last purchase
- Complain: 1 if the customer complained in the last 2 years, 0 otherwise
- MntWines: Amount spent on wine in last 2 years
- MntFruits: Amount spent on fruits in last 2 years
- MntMeatProducts: Amount spent on meat in last 2 years
- MntFishProducts: Amount spent on fish in last 2 years
- MntSweetProducts: Amount spent on sweets in last 2 years
- MntGoldProds: Amount spent on gold in last 2 years
- NumDealsPurchases: Number of purchases made with a discount
- AcceptedCmp1: 1 if customer accepted the offer in the 1st campaign, 0 otherwise
- AcceptedCmp2: 1 if customer accepted the offer in the 2nd campaign, 0 otherwise
- AcceptedCmp3: 1 if customer accepted the offer in the 3rd campaign, 0 otherwise
- AcceptedCmp4: 1 if customer accepted the offer in the 4th campaign, 0 otherwise
- AcceptedCmp5: 1 if customer accepted the offer in the 5th campaign, 0 otherwise
- Response: 1 if customer accepted the offer in the last campaign, 0 otherwise
- NumWebPurchases: Number of purchases made through the company’s website
- NumCatalogPurchases: Number of purchases made using a catalogue
- NumStorePurchases: Number of purchases made directly in stores
- NumWebVisitsMonth: Number of visits to company’s website in the last month

## 🔍 Cicle 1: Metrics
I started by making a baseline model so that I could have some metrics to evaluate the model's performance over the cicles.
The metrics that where chosen for this project where:
- **WSS (Within-Cluster Sum of Square):** a small sum of squares indicates a more compact cluster - meaning that the observations are closer within a cluster.
- **SS (Silhouette Score):** evaluates the similiarity of the observations in a cluster (if its closer to 1, means that the points belongs to the clusters they have been assigin, otherwise, if its closer to -1, means that the points should belong to other cluster).
![image](https://user-images.githubusercontent.com/82069205/152966261-3ccd10af-b8b4-42f4-a1c5-f8b69c6ecc4a.png)![image](https://user-images.githubusercontent.com/82069205/152966334-d817ae50-5053-4aee-9a53-61afe4165a9c.png)

## ⚙ Cicle 2: Descriptive Statistics and Feature Engineering.
In this cicle was made all the data description in order to better understand the missing values, data types and get some insights from the statistical description of the data. After that, I started the feature engineering to get new attributes from the originals ones given by the dataset and ran the metrics again, to see if it was impacted by the changes made. As long as the cicles advanced, new features were created and in each cicle the metrics were ran to see the differences. 
![image](https://user-images.githubusercontent.com/82069205/152966174-0aa09ab9-cc09-42d1-945c-4571c4886102.png)

## 📊 Cicle 3: RFM Model
For this cicle I implemented the RFM Model (Recency, Frequency and Monetary) to segment the customers into this 3 categories and see the metrics. The features were created based on the attributes I already had available in the dataset. 
![image](https://user-images.githubusercontent.com/82069205/152966015-6210f0e6-503c-42f5-8a81-f87fe71622f4.png)

## 📍 Cicle 4: Exploratory Data Analysis
Using the python library ProfileReport, I got some insights about the data and create some hypothesis to be validated. Puting an effort on finding out more information about the data, this phase of the project was crucial to get some insights and start to think about what would be the best features to be used for the model training.
![image](https://user-images.githubusercontent.com/82069205/152967040-dabe4ff7-b87f-48e5-9133-adb58b5a94e9.png)

## 🎲 Cicle 5: Data Preparation
In this phase I made all the data transformation needed to ajust the data for the model traning, using enconding for the categorical features, rescaling for the numerical ones and applied some transformation on the time nature features. 
![image](https://user-images.githubusercontent.com/82069205/152967441-43e72994-8ac4-488e-a4ca-d9dc909fa64b.png)

## 🤖 Cicle 6: Space Study
In order to get a better visualization of the data distribution and the clusters that might be formed

## 🔦 Cicle 7: Machine Learning Models

## ⁉ Cicle 8: Final Model

## 🛠 Cicle 9: Cluster's EDA

## 📲 Cicle 10: Deploy
