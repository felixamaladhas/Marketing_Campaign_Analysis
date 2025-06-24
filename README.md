# Marketing_Campaign_Analysis

# Objective
To analyze customer behavior using RFM segmentation and uncover purchase patterns using Market Basket Analysis in order to drive better marketing and business decisions.

* Segment customers into meaningful groups based on purchasing behavior.

* Identify frequent product combinations for cross-selling and upselling.

* Support business strategies with data-driven insights.


# Business Understanding
E-commerce platforms collect vast transaction data. However, raw data needs to be transformed into actionable insights to:

* Identify loyal customers and high-value segments.

* Understand customer retention patterns and churn risk.

* Recommend product bundles using association rules.

Two analytical methods are used:

* RFM Segmentation: Measures customer value.

* Market Basket Analysis: Reveals product purchasing relationships.


# Dataset Description
Source: Online Retail dataset (UCI Machine Learning Repository)

Records: ~540,000 transactions

Time Frame: December 2010 to December 2011

Fields:

* InvoiceNo, StockCode, Description

* Quantity, InvoiceDate, UnitPrice

* CustomerID, Country

Target region for analysis: UK and Germany

# Processing of Analysis
🔹 Data Preprocessing:
* Removed missing CustomerIDs, duplicate entries.
  
* Removed cancelled orders (negative quantity).

* Created TotalAmount = Quantity × UnitPrice.

🔹 RFM Segmentation:
* Calculated Recency, Frequency, and Monetary values.

* Scored and categorized customers into segments (Platinum, Gold, etc.).

* Applied K-Means clustering to group similar customers.

🔹 Market Basket Analysis:
* Transformed transaction data into a basket format.

* Applied Apriori and FP-Growth algorithms.

* Generated association rules based on support, confidence, and lift.
# Conclusion
Customer Segmentation helped identify high-value and at-risk customers for targeted marketing.

K-Means Clustering confirmed patterns in behavior and spending habits.

Market Basket Analysis revealed frequently bought-together items, ideal for product bundling.

These insights can guide:

* Loyalty programs

* Personalized recommendations

* Inventory and promotion planning
