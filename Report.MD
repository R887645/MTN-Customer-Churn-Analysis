# Introduction
This is an SQL project where I analyzed customer churn for MTN. I used Microsoft SQL Server to clean the dataset, calculate KPIs, and uncover churn drivers. 
My goal was to understand why customers leave and provide actionable recommendations for retention.

# Step 1: Data Cleaning
- I checked for duplicates using Customer_ID, MTN_Device, and Subscription_Plan — none were found.

- I verified revenue calculations and confirmed no missing values.

- I standardized churn status to “Yes” and “No.”

- I replaced NULLs in Reasons_for_Churn with “Not Applicable” for non-churned customers.

# Step 2: MTN Core KPIs (Data Analysis)

- Total Customers: 974

- Total Churned Customers: 284

- Churn Rate: 29.16%

- Retention Rate: 70.84%

- Average Revenue Per User (ARPU): ₦59,538.29

- Monthly Revenue Lost to Churn: ₦58,000,200

These KPIs gave me a clear picture of MTN’s customer base and the financial impact of churn.

# Step 3: Churn Trends (Monthly)

- January: 271 customers, 65 churned, churn rate 23.98%

- February: 450 customers, 142 churned, churn rate 31.56%

- March: 253 customers, 77 churned, churn rate 30.43%

- **My Insight: Churn increased after January, which suggests seasonal factors or onboarding issues.**

# Step 4: Why Customers Are Churning

- **By Device Type:** Mobile SIM Card users churned more than 5G Broadband Router users. This points to possible pricing or network issues.

- By Tenure: Long-term customers (12+ months) churned the most. This shows deeper dissatisfaction beyond the early months.

- High-Value Customers at Risk: I identified churned customers with above-average revenue. These are MTN’s most valuable clients and losing them has a big financial impact.
