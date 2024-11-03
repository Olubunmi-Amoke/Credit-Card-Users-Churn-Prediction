# Credit-Card-Users-Churn-Prediction

## Problem Statement
#### Business Context
The Thera bank recently saw a steep decline in the number of users of their credit card, credit cards are a good source of income for banks because of different kinds of fees charged by the banks like annual fees, balance transfer fees, and cash advance fees, late payment fees, foreign transaction fees, and others. Some fees are charged to every user irrespective of usage, while others are charged under specified circumstances.
Customers’ leaving credit cards services would lead bank to loss, so the bank wants to analyze the data of customers and identify the customers who will leave their credit card services and reason for same – so that bank could improve upon those areas
The objective of this project is to build a classification model that will help the bank improve its services so that customers do not renounce their credit cards

#### Data Description
CLIENTNUM: Client number. Unique identifier for the customer holding the account

Attrition_Flag: Internal event (customer activity) variable - if the account is closed then "Attrited Customer" else "Existing Customer"

Customer_Age: Age in Years

Gender: Gender of the account holder

Dependent_count: Number of dependents

Education_Level: Educational Qualification of the account holder - Graduate, High School, Unknown, Uneducated, College(refers to college student), Post-Graduate, Doctorate

Marital_Status: Marital Status of the account holder

Income_Category: Annual Income Category of the account holder

Card_Category: Type of Card

Months_on_book: Period of relationship with the bank (in months)

Total_Relationship_Count: Total no. of products held by the customer

Months_Inactive_12_mon: No. of months inactive in the last 12 months

Contacts_Count_12_mon: No. of Contacts in the last 12 months

Credit_Limit: Credit Limit on the Credit Card

Total_Revolving_Bal: Total Revolving Balance on the Credit Card

Avg_Open_To_Buy: Open to Buy Credit Line (Average of last 12 months)

Total_Amt_Chng_Q4_Q1: Change in Transaction Amount (Q4 over Q1)

Total_Trans_Amt: Total Transaction Amount (Last 12 months)

Total_Trans_Ct: Total Transaction Count (Last 12 months)

Total_Ct_Chng_Q4_Q1: Change in Transaction Count (Q4 over Q1)

Avg_Utilization_Ratio: Average Card Utilization Ratio

**What Is a Revolving Balance?**
If we don't pay the balance of the revolving credit account in full every month, the unpaid portion carries over to the next month. That's called a revolving balance

**What is the Average Open to buy?**
'Open to Buy' means the amount left on your credit card to use. Now, this column represents the average of this value for the last 12 months.

**What is the Average utilization Ratio?**
The Avg_Utilization_Ratio represents how much of the available credit the customer spent. This is useful for calculating credit scores.

**Relation b/w Avg_Open_To_Buy, Credit_Limit and Avg_Utilization_Ratio:**
( Avg_Open_To_Buy / Credit_Limit ) + Avg_Utilization_Ratio = 1

## Business Insights and Conclusions
Based on this project, below are insights and actionable business recommendations for Thera Bank’s credit card attrition problem:

**Insights**
A significant portion of attrited customers falls within lower income brackets and less education, such as high school or uneducated groups. These segments may be more sensitive to fees or credit limitations, influencing their decision to leave.

Higher attrition rates are seen among certain card types, particularly lower-tier cards.

Lower transaction counts and amounts are associated with higher attrition. This suggests that inactive or low-usage customers are more likely to leave, potentially because they do not see value in retaining the card.

Customers with fewer total relationships with the bank (e.g., only a single product like a credit card) also exhibit higher attrition rates. This indicates that loyalty and engagement may be lower for customers who only use a single service.

The best-performing model in terms of generalization to unseen data was the AdaBoost classifier with the original data, showing high recall and precision. This indicates the model’s effectiveness at identifying at-risk customers.

Features with high importance included transaction count and amount, average utilization ratio, and months of inactivity, suggesting these are strong indicators of attrition.


**Actionable Business Recommendations**
**Targeted Retention Campaigns:**
- For lower-income groups, consider promotional strategies that mitigate costs, such as fee reductions or introductory offers that highlight the value of card ownership. This may improve retention for cost-sensitive customers.
- Engagement Programs for Low Activity Users: Implement incentive programs (e.g., rewards for frequent usage, spending-based bonuses) for customers with lower transaction counts or inactive months to increase engagement and reduce attrition.
  
**Cross-Selling to Increase Relationship Depth:**
- Promote additional banking products (e.g., savings accounts, loans) to single-product customers. By increasing the number of relationships, customer loyalty may improve, and attrition may decrease. Tailor these offers to align with customer needs based on their profile and usage data.

**Enhanced Customer Education on Card Benefits:**
- Develop educational resources highlighting card benefits and rewards, especially targeting less-educated groups. Use email campaigns or app notifications to explain how card usage can maximize benefits and improve financial outcomes, possibly leading to increased retention.

