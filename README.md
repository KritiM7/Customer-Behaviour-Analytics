# Customer-Behaviour-Analytics

Project Overview:
This project focuses on identifying key drivers of customer behavior and revenue for a retail dataset. I combined SQL for analytical querying and Power BI for executive-level storytelling. The goal was to move beyond simple "total sales" metrics and instead identify Customer Lifetime Value (CLV), Churn Risk, and Operational Efficiency.

The Data Stack:
Python: Used for initial EDA and data cleaning to ensure consistency across the purchase_amount and age_group columns.
SQL (MySQL): Used to build complex business logic, including customer segmentation and revenue concentration queries.
Power BI: Developed a 3-page interactive dashboard to visualize findings for stakeholders.

Business Questions & SQL Logic: I focused on real-World business problems like Customer Segmentation.
Used CTEs and CASE logic to bucket users into New, Returning, and Loyal segments.
Revenue Concentration: Applied Window Functions (OVER(PARTITION BY...)) to calculate how much the top 3 products in each category contribute to total revenue.
Churn Risk: Developed logic to flag "Loyal" subscribers who haven't purchased in over 60 days.
VIP Identification: Found "Diamond VIPs" by filtering for customers by the average spend and high review ratings.

Dashboard Highlights: The Power BI dashboard is split into three strategic views:
1. Executive Overview: A high-level look at KPIs ($59.76 Avg Spend, 3.9K Customers). It highlights that while gender split is nearly equal, Young Adults are the primary revenue drivers.
2. Customer Loyalty & Retention: This page identifies that 88% of our customers are Active, but a small, high-value "High Churn Risk" group needs immediate marketing intervention. It also maps revenue by segment, showing that Loyal customers provide the vast majority of stable income.
3. Operational Analysis: Tells the "Cost of Satisfaction. Standard Shipping maintains higher satisfaction ratings than Express, suggesting we can optimize shipping costs without hurting the brand. Payment Efficiency Identified that PayPal and Credit Cards are the dominant payment methods, particularly for subscribers.
