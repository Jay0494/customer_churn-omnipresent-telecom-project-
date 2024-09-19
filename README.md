# customer_churn-omnipresent-telecom-project-
### Project Background: Churn and Retention Analysis

**Project Title**: Customer Churn and Retention Improvement Initiative

**Client Context**:
The client operates in the telecommunications sector, offering a variety of internet, phone, and related services. Despite having a broad customer base, the company is experiencing a customer churn rate of **26.54%**, meaning that over a quarter of their customers are leaving each year. This is a critical issue as it directly impacts their financial performance, with **$2.86 million in revenue lost annually** due to customer attrition. Additionally, certain segments of the customer base, such as those on month-to-month contracts and those paying via electronic checks, are showing significantly higher churn rates.

The company’s executive team has identified customer retention as a strategic priority, and the **retention manager** is tasked with developing data-driven strategies to reduce churn, improve customer loyalty, and minimize revenue loss. This project aims to support the retention team with an in-depth analysis of customer churn, establish KPIs for ongoing monitoring, and provide actionable insights for intervention.

**Objective**:
The primary objective of this project is to identify key drivers of customer churn, provide insights into customer retention trends, and recommend actionable strategies to improve retention and reduce churn. This will be achieved by analyzing customer behavior patterns, contract types, payment methods, and service-related issues. The final output will include a set of key performance indicators (KPIs) for the retention manager and a dashboard to track these metrics over time.

**Current Challenges**:
1. **High Churn Rate**: The company's churn rate of **26.54%** is considerably higher than industry benchmarks. Month-to-month contract customers and those using certain payment methods (e.g., electronic check) are the most likely to churn.
2. **Revenue Impact**: Churn is leading to substantial revenue loss, with **$2.86 million** in annual revenue lost from churned customers.
3. **Customer Satisfaction Issues**: There are a large number of administrative support tickets (3,632) compared to technical support tickets (2,955), indicating that issues related to billing, contracts, or customer service may be contributing to customer dissatisfaction.
4. **Service-Specific Churn**: Despite being a superior technology, **fiber optic customers** are leaving at a higher rate (41.89%) compared to DSL users, pointing to potential pricing, service quality, or customer experience issues.

**Scope of Work**:
- **Data Analysis**: Conduct a detailed analysis of the company's customer churn data to identify the main drivers of attrition. This will include segmentation by contract type, payment method, internet service type, and customer demographics.
- **KPI Development**: Establish key performance indicators (KPIs) that will allow the retention manager to monitor customer behavior trends, identify at-risk customer segments, and measure the effectiveness of retention strategies.
- **Dashboard Creation**: Design a user-friendly dashboard that will provide real-time insights into churn metrics, enabling the retention team to track performance, identify trends, and act proactively.
- **Recommendations**: Based on the data analysis, develop strategic recommendations to reduce churn, including contract optimization, payment method interventions, and improvements in customer service and experience.



![Screenshot_20240919-011804_Drive](https://github.com/user-attachments/assets/34212bf2-cb67-4178-8330-c809ee71bb3b)


## **TOOLS**
- PowerBi
- Power Query

## **Data Processing**
The data cleaning and modeling process using Power Query began with importing raw data From the Excel database. The first step was to clean the data by removing unnecessary columns that did not contribute to the analysis, streamlining the dataset for easier management. Missing data, such as null values, were handled by filling them with averages values.  

Each column was reviewed to ensure the correct data types were assigned preventing errors during analysis. Duplicate records were identified and removed to maintain accuracy. The data was then transformed, including normalizing metrics to enable fair comparisons across agents and time periods. Columns were split where needed, such as extracting the hour from a timestamp to analyze call patterns. In some cases, data sources were merged based on common keys, such as agent names or call IDs, to create a comprehensive dataset for analysis.

Once cleaned, the next step involved data modeling. Key relationships were created between the main fact tables, such as call logs and satisfaction ratings, and dimension tables like agent details and call times. These relationships, including "one-to-many" and "many-to-many" structures, ensured the data model reflected real-world hierarchies. Custom calculated columns and DAX measures were created for important metrics like average call duration per agent and total satisfaction score. This made the model dynamic, allowing for on-the-fly calculations in Power BI. 

Time intelligence was incorporated to analyze trends, such as peak call hours and month-over-month performance, by creating and linking a date table. To further optimize the model, unused columns were removed to reduce its size, improving performance in Power BI. Hierarchies were also established, making it easier to explore data and enable drill-down capabilities in the reports. This structured approach ensured the dataset was clean, well-organized, and ready for insightful analysis.
### Analysis of Churn Insights:

1. **Churn vs Retention Rate**:
   - **Churn Rate**: 26.54%
   - **Retention Rate**: 73.46%

   **Insight**: The company retains a healthy percentage of its customers, but a churn rate of over 25% is significant. This indicates that more than a quarter of customers are leaving, which could have a substantial impact on long-term revenue and profitability.

2. **Revenue Impact**:
   - **Total Revenue**: $16,056,168.7
   - **Revenue Lost from Churned Customers**: $2,862,926.90

   **Insight**: The company loses about 17.8% of its potential revenue due to churn. This shows a direct relationship between customer attrition and financial performance. Addressing churn effectively could reclaim a significant portion of this lost revenue.

3. **Tickets Analysis**:
   - **Admin Tickets**: 3,632
   - **Tech Tickets**: 2,955

   **Insight**: More admin tickets are raised compared to tech tickets, indicating potential customer dissatisfaction or confusion with administrative aspects (billing, account management) over technical issues. Streamlining administrative processes might reduce friction points for customers.

4. **Revenue by Contract Type**:
   - **Two-Year Contracts**: $6,283,253.7
   - **One-Year Contracts**: $4,467,053.5
   - **Month-to-Month**: $5,305,861.5

   **Insight**: The highest revenue comes from two-year contracts, followed by month-to-month, then one-year. This indicates that longer-term contracts may be more lucrative and stable, but month-to-month offers flexibility. The company may benefit from offering incentives for longer-term commitments to drive up revenue stability.

5. **Churn Rate by Contract Type**:
   - **Month-to-Month**: 42.71%
   - **One-Year**: 11.27%
   - **Two-Year**: 2.83%

   **Insight**: The churn rate for month-to-month contracts is very high, whereas longer-term contracts (one- and two-year) have much lower churn rates. This suggests that encouraging customers to commit to longer contracts could significantly reduce churn.

6. **Churn Rate by Payment Method**:
   - **Electronic Check**: 45.29%
   - **Mailed Check**: 19.11%
   - **Bank Transfer**: 16.71%
   - **Credit Card**: 15.24%

   **Insight**: Customers who use electronic checks have the highest churn rate, while those paying via credit card or bank transfer are less likely to churn. This may suggest a correlation between payment method convenience and customer loyalty. Encouraging customers to switch to more stable and automatic payment methods could reduce churn.

7. **Churn Rate by Internet Service Type**:
   - **Fiber Optic**: 41.89%
   - **DSL**: 18.96%
   - **No Internet Service**: 7.40%

   **Insight**: Fiber optic customers have the highest churn rate despite it being a faster, more reliable service. This suggests that other factors like price, customer service, or competition might be affecting these customers' decisions to leave.

8. **Churn by Multiple Lines**:
   - **Multiple Lines**: 28.61%
   - **No Multiple Lines**: 25.04%
   - **No Phone Service**: 24.93%

   **Insight**: Customers with multiple lines tend to have a slightly higher churn rate. This could indicate that managing multiple services adds complexity and frustration, leading to higher churn.

9. **Dependents and Churn**:
   - **Customers without dependents**: 66.94%
   - **Customers with dependents**: 33.06%

   **Insight**: A larger proportion of churned customers do not have dependents, suggesting that families may be more stable and less likely to churn. This could inform targeted retention strategies focused on households without dependents.

### Recommendations:

1. **Promote Long-Term Contracts**: 
   Encourage customers to switch to one- or two-year contracts by offering discounts, perks, or loyalty rewards. This could significantly reduce churn.

2. **Targeted Payment Method Interventions**: 
   Customers using electronic checks have a notably higher churn rate. Offering incentives (e.g., discounts) to switch to automatic payment methods like credit cards or bank transfers could improve retention.

3. **Improve Customer Experience with Fiber Optic Services**:
   Since fiber optic customers have the highest churn despite using superior technology, investigate service quality, pricing, and customer service issues specific to these customers. Improved communication and support may help retain them.

4. **Focus on Administrative Efficiency**:
   The higher volume of administrative tickets indicates potential issues with billing, contracts, or account management. Streamlining these processes and improving the customer experience in this area may reduce churn.

5. **Retention Programs for Customers Without Dependents**:
   Since individuals without dependents are more likely to churn, tailor specific retention programs (e.g., personalized offers, product bundles) targeting single individuals or smaller households.

By implementing these strategies, the company can address key drivers of churn and improve both customer retention and overall financial performance.
