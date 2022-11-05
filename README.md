# Telco Customer Churn Analysis
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
