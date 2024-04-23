# Bank Customer Churn Analysis

In this project, we aim to perform data analysis on bank customer data to identify the reasons why customers leave the bank. Tools used for the analysis are Power BI, SQL, and Excel.

## Table of Contents
- [Project Overview](#project-overview)
- [Problem Statement](#problem-statement)
- [Data Source](#data-source)
- [Data Cleaning/Preparation](#data-cleaningpreparation)
- [Live Dashboard](#live-dashboard)
- [Inferences](#inferences)
- [Recommendations](#recommendations)
  
### Project Overview
1. The aim of this project is to analyze bank customer data to identify the factors contributing to customer churn using Power BI, SQL, and Excel.
2. To gather valuable insights from the analysis to understand patterns, trends, and correlations associated with bank customer data.
3. To provide recommendations to the bank to mitigate churn. It allows banks to address customer needs, improve retention strategies, and save costs associated with acquiring new customers. Identifying at-risk customers allows banks to implement personalized retention strategies, improving customer experience, and reducing attrition rates.

### Problem Statement
The bank is facing a significant challenge with high churn rates and aims to reduce costs linked to customer acquisition. Understanding the reasons behind customer churn is pivotal for tailoring services and implementing targeted retention efforts. This allows the bank to address customer needs, refine retention strategies, and identify at-risk customers for personalized retention strategies.

### Data Source
- Domain: Banking Domain
- Dataset Name: Bank_Churn.csv, ActiveCustomer.xlsx, CreditCard.xlsx, CustomerInfo.csv, ExitCustomer.xlsx, Gender.xlsx, Geography.xlsx
- Dataset Type: Excel and CSV Datatypes
- Dataset Size: 10,000 customers' data spanning 4 years.

### Data Dictionary (The complete understanding of Business)

1)	**RowNumber**: corresponds to the record (row) number and has no effect on the output.

2)	**CustomerId**: contains random values and has no effect on customer leaving the bank.

3)	**Surname**: the surname of a customer has no impact on their decision to leave the bank.

4)	**CreditScore**: can have an effect on customer churn, since a customer with a higher credit score is less likely to leave the bank.
   - Credit score ranges:
     - Excellent: 800–850
     - Very Good: 740–799
     - Good: 670–739
     - Fair: 580–669
     - Poor: 300–579

5)	**Geography**: a customer’s location can affect their decision to leave the bank.

6)	**Gender**: it’s interesting to explore whether gender plays a role in a customer leaving the bank.

7)	**Age**: this is certainly relevant, since older customers are less likely to leave their bank than younger ones.

8)	**Tenure**: refers to the number of years that the customer has been a client of the bank. Normally, older clients are more loyal and less likely to leave a bank.

9)	**Balance**: also a very good indicator of customer churn, as people with a higher balance in their accounts are less likely to leave the bank compared to those with lower balances.

10)	**NumOfProducts**: refers to the number of products that a customer has purchased through the bank.

11)	**HasCrCard**: denotes whether or not a customer has a credit card.
    - 1 represents credit card holder
    - 0 represents non-credit card holder

12)	**IsActiveMember**: active customers are less likely to leave the bank.
    - 1 represents Active Member
    - 0 represents Inactive Member

13)	**Estimated Salary**: as with balance, people with lower salaries are more likely to leave the bank compared to those with higher salaries.

14)	**Exited**: whether or not the customer left the bank.
    - 0 represents Retain   (Still they are with the bank)
    - 1 represents Exit

15)	**Bank DOJ**: date when the Customer associated/joined with the bank

### Data Cleaning/Preparation

- Checked for presence of duplicates and eliminated them.
- Removing irrelevant columns which does not associated with customer churn.
- Data type standardization.
- Formatting dates for consistency.
- Formatted numerical data for consistency.
- Handling the text values and removed special characters in name.
- Handled null values.



  
### Data Modelling:
Established star schema relationship between fact table and dimension tables in Power Pivot.
![DataModel(CustomerChurn)](https://github.com/hello-mr-vishu/Bank-Customer-Churn-Analysis/assets/130839613/d60c19fe-f976-45be-bf56-85a173ba25a6)


### End To End - TASKS Performed - Life Cycle of a Data Analyst

- Requirement Gathering (BRD / FRD)
- Data Collections (Database / CSV/ Excel)
- Data Modelling
- Data Cleaning / Data Pre-processing
- UI Report (Charts / Custom Charts)
- Additional Information (DAX Calculations)
- RLS

• Created a Workspace

• Published
• Dashboard
• Gateway
• Schedule Refresh
• Added Roles, Subscribe, alerts
• Shared the Report
• Created App and Shared
![HomePage](https://github.com/hello-mr-vishu/Bank-Customer-Churn-Analysis/assets/130839613/d8d39563-264d-437e-9bd2-1755d9ee3f75)


### Report
[Report](https://app.powerbi.com/links/UdvwbggkVD?ctid=63b5c61a-66d9-46b2-9b8d-10c275a4acac&pbi_source=linkShare)

 ### Live Dashboard
 [Power BI Dashboard](https://app.powerbi.com/groups/c9aa63dc-18b2-4261-96bd-209a9efdd76a/dashboards/f08ebaf2-64a1-4c1e-88b8-bb14791dbd92?ctid=63b5c61a-66d9-46b2-9b8d-10c275a4acac&pbi_source=linkShare)


### Inferences
Inferences from the analysis:
1. Total customers associated with the bank are 10,000.
2. Churn Rate is 20.37%. Which is higher than the healthy range, churn rate of 5-7% annually is considered average in the banking industry. So the bank should consider this as a serious problem and take necessary actions.
3. Retention Rate 79.63%. High retention rate indicates customer satisfaction and loyalty. Anything above 90% might be considered healthy.
4. Active Customer Rate 51.51%. Desired range for active customer rate is above 70-80%. These desired ranges can vary based on the bank's services and customer engagement strategies. Inactive Customers have a higher churn rate.
6. Credit Card Holder Rate is 70.55%. Bank is doing good in this case. Typically, a rate higher than 50-60% might be considered good, but this can vary widely. But, churn rate is high in case of the credit card holders. People with fair and poor credit score are leaving the bank. 
7. Customers have a varying number of products, typically ranging from 1 to 4. Products Per Customers is 1.53. Around 3-4 products per customer are often seen as a good benchmark. Most of customers has 1 or 2 products and churn rate is more in that range.
8. Average Tenure is 5 Years, Indicating the level of loyalty and the bank's ability to retain its customer base. Most of the customers are leaving the bank within 4 to 5 years.
9. Average age 39. Churn rate is high in the case of the Late Adulthood age group. 
10. Average Balance Per Customer is around 75k. Customers with a higher balance churn more which would be worrying to the bank as this impacts their source of loan capital.
11. Churn Rate is minimum in Year 2016 that is 19.27% and maximum in year 2017 that is 22.35%. Also, we have forecasted the Churn rate for the next four quarters predicting churn rate between lower bound 15 or 16% and the upper bound is 24 to 25% with a 95% confidence level.
12. Churn rate is high in female compared to male even though there are more male customers.
13. Churn Rate is highest in Germany that is 32.44% and for both France and Spain churn rate is around 16%.

### Recommendations:
1. Enhance customer service, resolving customers' issues, offer personalized experiences to increase satisfaction.
2. Implement loyalty programs, rewards for long-term customers to reduce churn.
3. Regularly engage with customers via multiple channels, offering relevant updates and personalized offers.
4. Collect and act on customer feedback to address pain points and enhance overall satisfaction
5. Encourage active participation in banking activities, offer exclusive benefits, and personalize services based on customer behavior.
6. Upselling and Cross-Selling; Train staff to recommend complementary products or services to existing customers based on their profiles and behavior.
7. Customer Segmentation: Segment customers based on behavior and preferences, offering tailored packages to each segment. Like


