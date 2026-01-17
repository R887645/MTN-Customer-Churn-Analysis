# Introduction
This is an SQL project where I analyzed customer churn for MTN. I used Microsoft SQL Server to clean the dataset, calculate KPIs, and uncover churn drivers. 
My goal was to understand why customers leave and provide actionable recommendations for retention.

![My Image Description](https://github.com/R887645/MTN-Customer-Churn-Analysis/blob/main/14228fe1-eeee-451f-9e2c-2db71aaed605-0.jpg?raw=true)

# Step 1: Data Cleaning
- I checked for duplicates using Customer_ID, MTN_Device, and Subscription_Plan — none were found.

- I verified revenue calculations and confirmed no missing values.

- I standardized churn status to “Yes” and “No.”

- I replaced NULLs in Reasons_for_Churn with “Not Applicable” for non-churned customers.

In my analysis, I noticed that some customers appeared multiple times in the dataset because the same person purchased different devices. These were not true duplicates — deleting them would have removed important information needed for analysis.

To handle this correctly, I added a new unique key called RecordID. This ensured that:

- Every row had a unique identifier.

- Customer data remained intact.

I could still analyze multiple purchases by the same customer without losing detail. This step preserved the richness of the dataset while maintaining accuracy in the analysis.

![My Image Description](https://github.com/R887645/MTN-Customer-Churn-Analysis/blob/main/14228fe1-eeee-451f-9e2c-2db71aaed605-4.jpg?raw=true)

# Step 2: MTN Core KPIs (Data Analysis)

- Total Customers: 974

- Total Churned Customers: 284

- Churn Rate: 29.16%

- Retention Rate: 70.84%

- Average Revenue Per User (ARPU): ₦59,538.29

- Monthly Revenue Lost to Churn: ₦58,000,200

These KPIs gave me a clear picture of MTN’s customer base and the financial impact of churn.

![My Image Description](https://github.com/R887645/MTN-Customer-Churn-Analysis/blob/main/14228fe1-eeee-451f-9e2c-2db71aaed605-6.jpg?raw=true)

# Step 3: Churn Trends (Monthly)

- January: 271 customers, 65 churned, churn rate 23.98%

- February: 450 customers, 142 churned, churn rate 31.56%

- March: 253 customers, 77 churned, churn rate 30.43%

- **My Insight: Churn increased after January, which suggests seasonal factors or onboarding issues.**

![My Image Description](https://github.com/R887645/MTN-Customer-Churn-Analysis/blob/main/14228fe1-eeee-451f-9e2c-2db71aaed605-9.jpg?raw=true)

# Step 4: Why Customers Are Churning

- **By Device Type:** Mobile SIM Card users churned more than 5G Broadband Router users. This points to possible pricing or network issues.

- **By Tenure:** Long-term customers (12+ months) churned the most. This shows deeper dissatisfaction beyond the early months.

- **High-Value Customers at Risk:** I identified churned customers with above-average revenue. These are MTN’s most valuable clients, and losing them has a big financial impact.

![My Image Description](https://github.com/R887645/MTN-Customer-Churn-Analysis/blob/main/14228fe1-eeee-451f-9e2c-2db71aaed605-11.jpg?raw=true)

# Step 5: Top Reasons for Churn

- High Call Tariffs – 54 customers

- Better Offers from Competitors – 52 customers

- Poor Network – 45 customers

- Costly Data Plans – 40 customers

- Poor Customer Service – 34 customers

- Fast Data Consumption – 32 customers

- Relocation – 27 customers

**My Insight: The top two reasons (high call tariffs and competitor offers) together account for over 100 churned customers, making pricing and competitive positioning the most urgent issues to address.**

![My Image Description](https://github.com/R887645/MTN-Customer-Churn-Analysis/blob/main/14228fe1-eeee-451f-9e2c-2db71aaed605-14.jpg?raw=true)

# Key Recommendations 

Based on my analysis, I recommend that MTN should try to:

- **Review pricing and call tariffs:** Since high tariffs and costly data plans are top churn reasons, MTN should try to adjust pricing strategies or introduce competitive bundles.

- **Improve network quality:** Poor network performance is a major churn driver. I recommend that MTN invest in infrastructure upgrades, especially in regions with high churn.

- **Focus on customer onboarding and support:** With churn rising after the first month, MTN should try to strengthen onboarding programs and customer service to reduce early exits.

- **Protect high-value customers:** I recommend creating loyalty programs or VIP support for customers with above-average revenue, as losing them has the biggest financial impact.

![My Image Description](https://github.com/R887645/MTN-Customer-Churn-Analysis/blob/main/14228fe1-eeee-451f-9e2c-2db71aaed605-15.jpg?raw=true)

This project demonstrates my ability to clean and analyze customer data using SQL, calculate KPIs, and uncover churn drivers. I translated the findings into actionable recommendations that can help MTN make better decisions about pricing, customer experience, and retention strategies.

I believe this analysis can also help other telecommunication companies facing similar churn challenges. By applying these insights, they can make better decisions and proactively address customer dissatisfaction before it leads to revenue loss.
