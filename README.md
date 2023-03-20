# Customer Churn Prediction 
## A Supervised Machine Learning Project

### DOMAIN: Telecom

### PROJECT OBJECTIVE: 
Build a model that will help to identify the potential customers who have a higher probability to churn.This help the company to understand the pinpoints and patterns of customer churn and will increase the focus on strategizing customer retention.

### DATA DESCRIPTION: 
Each row represents a customer, each column contains customer’s attributes described on the column Metadata. 
The data set includes information about:
- Customers who left within the last month : the column is called Churn (target)
- Services that each customer has signed up for : phone, multiple lines, internet, online security, onlinebackup,device protection, tech support, and streaming TV and movies
- Customer account information : how long they’ve been a customer, contract, payment method, paperless billing, monthly charges, and total charges
- Demographic info about customers : gender, age range, and if they have partners and dependentsPROJECT OBJECTIVE: Build a model that will help to identify the potential customers who have a higher probability to churn. This will help the company to understand the pinpoints and patterns of customer churn and will increase the focus on strategizing customer retention.

### Attributes :
(Total 21 attributes)

- CustomerID	
- Gender	
- SeniorCitizen	
- Partner	
- Dependents	
- Tenure	
- PhoneService	
- MultipleLines	
- InternetService	
- OnlineSecurity	
- OnlineBackup	
- DeviceProtection	
- TechSupport	
- StreamingTV	
- StreamingMovies	
- Contract	
- PaperlessBilling	
- PaymentMethod	
- MonthlyCharges	
- TotalCharges	
- Churn

### Steps taken in the Project:
1. Importing the datasets 'TelecomCustomerChurn1' and 'TelecomCustomerChurn2' in MYSQL server using MYSQL workbench.
   Then importing them into jupyter notebook and merging all datasets into one.
2. Data Cleansing:
   - Dropping any missing and duplicate values
   - Dropping redundant columns
   - Encoding categorical variables
3. Exploratory Data Analysis:
   - Detailed statistical analysis on the data.
   - Detailed univariate, bivariate, and multivariate analysis
4. Data Preparation for model building: 
   - Separating target (Churn) and predictor variables.
   - Spliting the dataset into 70% train and 30% test
   - Standardizing the columns using z-score scaling approach.
5. Model training, and testing:
   We trained 3 models:
   - Logistic regression:
     - Train Accuracy = 80.7
     - Test Accuracy = 80.4
   - KNN:
     - Train Accuracy = 99.8
     - Test Accuracy = 74.4
   - Naive Bayes:
     - Train Accuracy = 69.4
     - Test Accuracy = 70.6
 6. Selecting Best Trained Model:
    On the basis of Train and Test accuracies as well as other performance metrics like precision, recall and f1-score we were able to conclude that the best trained       model is :
    
    Logistic regression:
     - Train Accuracy = 80.7
     - Test Accuracy = 80.4

### CONCLUSIONS:
    Concluding this case-study we can say that for selecting our machine learning model we should take care of the following:
    - An imbalance in dataset should be avoided but if it is present then we should not select our model based purely on overall accuracy but observe other metrics as     well.
    - When we have to consider imbalance dataset only, the accuracies alone can be misleading for comparing various ML models.
    - We should also comapare train and test accuracies to check if there is overfitting or underfitting in our model.
