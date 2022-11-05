# Telco Customer Churn Analysis
# Data Cleansing
- Data cleansing is the process of identifying and resolving corrupt, inaccurate, or irrelevant data. 
- Common inaccuracies in data include missing values, misplaced entries, and typographical errors. In some cases, data cleansing requires certain values to be filled in or corrected, while in other instances, the values will need to be removed altogether.

# Exploratory Data Analysis
How many churn customers and no churn customers?

![churn no churn](https://user-images.githubusercontent.com/113869968/200099130-6e88407e-0e3a-4a90-9af0-bfe3fd6c3dbe.jpg)
No Churn customers there are as much as 73.46%, while churn customers there are as much as 26.54%.

How many churn customers based on gender?

![gender](https://user-images.githubusercontent.com/113869968/200099132-34a88388-e541-4858-b52f-4706f669a99d.jpg)

Most churn customers are female who are 11.44%. Male churn customers are as many as 11.39% and 3.71% are churn customers that their gender is not known. While the remaining 73.46% are no churn customers.

How many churn customers based on senior citizen?

![senior](https://user-images.githubusercontent.com/113869968/200099136-7e411cc1-e6f0-4ae9-b02b-c1cea244fddf.jpg)

From churn customers, the majority are not seniors, which is as much as 17%. 5.84% other are senior citizens and 3.71% are churn customers who are unknown. While the remaining 73.45% are no churn customers.

How many churn customers based on dependents?

![dependents](https://user-images.githubusercontent.com/113869968/200099131-ed954e46-9081-434f-8928-fc152b935e4f.jpg)

18.83% of customers are churn customers and have no dependents. While 4% of them have dependents and 3.71% are not known. While the remaining 73.47% are no churn customers.

How many churn customers based on partner?

![partner](https://user-images.githubusercontent.com/113869968/200099135-33538da0-a6cb-44b1-b02a-131b98192851.jpg)

Most churn customers are customers who don't have a partner, that is as much as 14.65% of all numbers customers. 8.18% have a partner and 3.71% are not known. While the remaining 73.46% are no churn customers.

Is there multicolinierity between variables?

![multi](https://user-images.githubusercontent.com/113869968/200099134-be9d98f7-3e9b-4c5a-8134-3816faa3c2f7.jpg)

There is a multicollinearity between tenure with Total Charges and Monthly Charges with Total Charges. Then it must be removed one of the variables from the three variables above before modeling
