# Telco Customer Churn Analysis

# Machine Learning Workflow
- Use Case
  - Objective Statement
  - Challenges
  - Analytic Method/Technique
  - Business Benefit
  - Expected Outcome
- Business Understanding
- Data Understanding
- Data Preparation
- Data Profiling
- Data Cleansing
- Data Exploration
- Feature Engineering
- EDA
- Modeling using Logistic Regression
- AUC/ROC
- Build a Model with Cross Validation
- Hyperparameter Tuning in Logistic Regression
- Oversampling with SMOTE
- Evaluate Model
- Result
- Recommendation

# Use Case
- Objective Statement:
  - To get insight into what type gender who churn and no churn.
  - To gain insight into senior citizens who churn and no churn.
  - To gain insight into churn and no churn customers whether the customer has a partner or has dependents.
  - To gain insight into churn and no churn customers based on how long the customer has worked in the company.
  - To gain insight into churn and no churn customers based on how many customers use Internet Service, Online Security, Multiple Lines, Online Backup, Device Protection, Tech Support, Streaming TV, Movie Streaming, Payment Methods, and Paperless Billing facilities.
  - To get insight about what type based on customer contract churn and no churn.
  - To get insight about how long customers churn, monthly subscription fees, and the total cost they spend on services.
  - To get insight about customer churn analysis.
  - To create modeling with Machine Learning to predict customer churn.

- Challenges:
  - There are some variables containing many missing values
  - There are some inappropriate data types
  - There is multicolinerity on some variables

- Methodology / Analytic Technique:
  - Descriptive analysis
  - Graph analysis
  - Modelling using Logistic Regression
  
- Business Benefit:
  - Helping Business Development Team to create product differentiation based on the characteristic for each customer.
  - Know how to treat customers with spesific criteria, especially between those who are still subscribing and unsubscribed.

- Expected Outcome:
  - Know how many customers based on gender type who churn and no churn.
  - Know how many customers based on senior citizens who churn and no churn.
  - Know how many customers based on churn and no churn customers whether the customer has a partner or has dependents.
  - Know how many customers based on churn and no churn customers based on how long the customer has worked in the company.
  - Know how many customers based on churn and no churn customers based on how many customers use Internet Service, Online Security, Multiple Lines, Online Backup, Device Protection, Tech Support, Streaming TV, Movie Streaming, Payment Methods, and Paperless Billing facilities.
  - Know how many customers based on type customer contract churn and no churn.
  - Know how long customers churn, monthly subscription fees, and the total cost they spend on services.
  - Know customer churn analysis.
  - Create modeling with Machine Learning to predict customer churn
  
# Business Understanding
- Data telco is a company engaged in telecommunication and internet services to make easier for consumers to communicate remotely and surf the internet more easily with offers several services such as time contracts, and various types of services.
- This case has some business question using the data:
  - How many customers based on gender type who subscribed and unsubscribed?
  - How many customers based on senior citizens who subscribed and unsubscribed?
  - How many customers based on subscribed and unsubscribed customers whether the customer has a partner or has dependents?
  - How many subscribed and unsubscribed customers based on how long the customer has worked in the company?
  - How many subscribed and unsubscribed customers based on how many customers use Internet Service, Online Security, Multiple Lines, Online Backup, Device Protection, Tech Support, Streaming TV, Movie Streaming, Payment Methods, and Paperless Billing facilities?
  - How many customers based on type customer contract unsubscribe and subscribe?
  - How long customers subscribe, monthly subscription fees, and the total cost they spend on services?
  - How about customer churn analysis?
  -  How to create modeling with Machine Learning to predict customer churn?

# Data Understanding
- Data of Telecom Customer with 21 columns and 7043 rows
- Source Code : https://www.kaggle.com/datasets/blastchar/telco-customer-churn

- Data Dictionary :  
  - customerId : Customer number uniquely assigned to each customer.
  - gender : gender of customer
  - SeniorCitizen : Whether the customer is a senior citizen or not (1, 0)
  - partner : Whether the customer has a partner or not (Yes, No)
  - Dependets : Whether the customer has dependents or not (Yes, No)
  - tenure : Number of months the customer has stayed with the company
  - PhoneService : Whether the customer has a phone service or not (Yes, No)
  - MultipleLines : Whether the customer has multiple lines or not (Yes, No, No phone service)
  - InternetService : Customer’s internet service provider (DSL, Fiber optic, No)
  - OnlineSecurity : Whether the customer has online security or not (Yes, No, No internet service)
  - OnlineBackup : Whether the customer has online backup or not (Yes, No, No internet service)
  - DeviceProtection : Whether the customer has device protection or not (Yes, No, No internet service)
  - TechSupport : Whether the customer has tech support or not (Yes, No, No internet service)
  - StreamingTV : Whether the customer has streaming TV or not (Yes, No, No internet service)
  - StreamingMovies : Whether the customer has streaming movies or not (Yes, No, No internet service)
  - Contract : The contract term of the customer (Month-to-month, One year, Two year)
  - PaperlessBilling : Whether the customer has paperless billing or not (Yes, No)
  - PaymentMethod : The customer’s payment method (Electronic check, Mailed check, Bank transfer (automatic), Credit card (automatic))
  - MonthlyCharges : The amount charged to the customer monthly
  - TotalCharges : The total amount charged to the customer
  - Churn : The customer churn status (1 - Yes, 0 - No) 

# Data Preparation
- Code Used:
  - Python Version: 3.7.15
  - Packages: Pandas, Numpy, Matplotlib, Seaborn, Sklearn, and Warnings

# Data Profiling
Data profiling is the process of reviewing source data, understanding structure, content and interrelationships, and identifying potential for data projects.

# Data Cleansing
- Data cleansing is the process of identifying and resolving corrupt, inaccurate, or irrelevant data. 
- Common inaccuracies in data include missing values, misplaced entries, and typographical errors. In some cases, data cleansing requires certain values to be filled in or corrected, while in other instances, the values will need to be removed altogether.

# Exploratory Data Analysis
- How many churn customers and no churn customers?

  ![churn no churn](https://user-images.githubusercontent.com/113869968/200099130-6e88407e-0e3a-4a90-9af0-bfe3fd6c3dbe.jpg)

  No Churn customers there are as much as 73.46%, while churn customers there are as much as 26.54%.

- How many churn customers based on gender?

  ![gender](https://user-images.githubusercontent.com/113869968/200099132-34a88388-e541-4858-b52f-4706f669a99d.jpg)

  Most churn customers are female who are 11.44%. Male churn customers are as many as 11.39% and 3.71% are churn customers that their gender is not known. While the  remaining 73.46% are no churn customers.

- How many churn customers based on senior citizen?

  ![senior](https://user-images.githubusercontent.com/113869968/200099136-7e411cc1-e6f0-4ae9-b02b-c1cea244fddf.jpg)

  From churn customers, the majority are not seniors, which is as much as 17%. 5.84% other are senior citizens and 3.71% are churn customers who are unknown. While the remaining 73.45% are no churn customers.

- How many churn customers based on dependents?

  ![dependents](https://user-images.githubusercontent.com/113869968/200099131-ed954e46-9081-434f-8928-fc152b935e4f.jpg)

  18.83% of customers are churn customers and have no dependents. While 4% of them have dependents and 3.71% are not known. While the remaining 73.47% are no churn customers.

- How many churn customers based on partner?

  ![partner](https://user-images.githubusercontent.com/113869968/200099135-33538da0-a6cb-44b1-b02a-131b98192851.jpg)

  Most churn customers are customers who don't have a partner, that is as much as 14.65% of all numbers customers. 8.18% have a partner and 3.71% are not known. While the remaining 73.46% are no churn customers.

- Is there multicolinierity between variables?

  ![multi](https://user-images.githubusercontent.com/113869968/200099134-be9d98f7-3e9b-4c5a-8134-3816faa3c2f7.jpg)

  There is a multicollinearity between tenure with Total Charges and Monthly Charges with Total Charges. Then it must be removed one of the variables from the three variables above before modeling

# Feature Engineering
Feature engineering is the process of selecting, manipulating, and transforming raw data into features that can be used for creating a predictive model using Machine learning or statistical Modelling.

- One-hot Encoding
One-hot encoding is a process of converting categorical data variables so they can be provided to machine learning algorithms to improve predictions.
The Python library Pandas provides a function called get_dummies to enable one-hot encoding
- map() function
To convert numerical data variables can use the map() function
- Scaling
  - Feature scaling is about transforming the values of different numerical features to fall within a similar range like each other. The feature scaling is used to prevent the supervised learning models from getting biased toward a specific range of values.
  - StandardScaler is a class from sklearn.preprocessing which is used for standardization.
  - Standardization is used to center the feature columns at mean 0 with a standard deviation of 1 so that the feature columns have the same parameters as a standard normal distribution.

# Result
- No Churn customers there are as much as 73.46%, while churn customers there are as much as 26.54%.
- Most churn customers are female who are 11.44%. Male churn customers are as many as 11.39% and 3.71% are churn customers that their gender is not known. While the remaining 73.46% are no churn customers.
- From churn customers, the majority are not seniors, which is as much as 17%. 5.84% other are senior citizens and 3.71% are churn customers who are unknown. While the remaining 73.45% are no churn customers.
- Most of the churn customers are customers who use Fiber Optics internet services are 15.75%. 5.69% DSL users, 3.71% unknown, and 1.39% did not have internet services. While the remaining 73.46% are no churn customers.
- Most churn customers are customers who use electronic transactions (paperless billing) that are 19.88% while 6.66% were not paperless billing users. The remaining 73.46% are no churn customers.
- 18.83% of customers are churn customers and have no dependents. While 4% of them have dependents and 3.71% are not known. While the remaining 73.47% are no churn customers.
- Most churn customers are customers who don't have a partner, that is as much as 14.65% of all numbers customers. 8.18% have a partner and 3.71% are not known. While the remaining 73.46% are no churn customers.
- 24.12% of customers are churn customers and have phone services. while 2.41% were not have phone service. The remaining 73.46% are no churn customers.
- Most churn customers are customers who have multiple lines, that are 10.46% of customers. 10.28% did not have multiple lines, 3.71% of it is unknown, and 2.09% did not have phone services. While the remaining 73.47% are no churn customers.
- Most churn customers are customers who do not have online security, which is 17.88% customers. 3.56% have online security, 3.71% of them are unknown, and 1.39% do not have internet services. The remaining 73.46% are no churn customers.
- Most churn customers are customers who do not have online backup, which is 15.15% customers. 6.29% have online backup, 3.71% of them are unknown, and 1.39% do not have internet services. The remaining 73.46% are no churn customers.
- Most churn customers are customers who have no device protection, which is 14.81% of customers. 6.63% of it have device protection, 3.71% of them are unknown, and 1.39% do not have internet services. The remaining 73.46% are no churn customers.
- Most churn customers are customers who don't have technical support services, that is 17.54% of customers. 3.9% of them have a technical support, 3.71% of them are unknown, and 1.39% do not have internet services. The remaining 73.46% are no churn customers.
- Most churn customers are customers who do not use Streaming TV services, which is 11.39% of customers. 10.05% of it uses streaming TV services, 3.71% of which are unknown, and 1.39% have no internet services. The remaining 73.46% are no churn customers.
- Most churn customers are customers who do not use Streaming Movies service, which is 11.54% of customers. 9.9% of it using Streaming Movies service, 3.71% of it is unknown, and 1.39% have no internet services. The remaining 73.46% are no churn customers.
- Most churn customers are customers who have monthly contracts, that are 23.50% of customers. 2.36% of it had a one-year contract, and 0.68% had a two-year contract. The remaining 73.46% are no churn customers.
- 15.21% of customers are churn customers and use Elektronic Check payments method. 4.37% of them used Mailed check, 3.66% of them use bank transfers, and 3.29% are churn customers and use credit cards. The remaining 73.46% are no churn customers.
- Most churn customers are customers whose tenure is only 1 month with an average is 18 months.
- Most churn customers on average are customers who spend 74.4 per month.
- The average total costs incurred by no churn customers is 1531.8 where it is smaller than a no churn customers.
- After creating modeling with logistics regression, then the evaluation is made using the AUC/ROC. It can be concluded that the resulting model does not overfit because the AUC train is obtained by 83.53% and the test earned by 85.99%, where the difference is no more than 0.05.
