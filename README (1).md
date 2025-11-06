
# O-list-E-Commerce-Analytics

Analyzes Olist’s e-commerce data to explore customer patterns, sales performance, payment behavior, and delivery efficiency through Python-based analytics and visual storytelling.

# Table Content :
1. [Overview](https://github.com/KRATIKA-HUB/O-list-E-Commerce-Analytics/blob/main/README%20(1).md#overview)
2. [Business Problem Statement](https://github.com/KRATIKA-HUB/O-list-E-Commerce-Analytics/blob/main/README%20(1).md#business-problem-statement-)
3. [Dataset Overview](https://github.com/KRATIKA-HUB/O-list-E-Commerce-Analytics/blob/main/README%20(1).md#dataset-overview-)
4. [Tools & Techniques](https://github.com/KRATIKA-HUB/O-list-E-Commerce-Analytics/blob/main/README%20(1).md#tools--techniques-)
5. [Table Structure](https://github.com/KRATIKA-HUB/O-list-E-Commerce-Analytics/blob/main/README%20(1).md#table-structure-)







## Overview:
This project provides a comprehensive analysis of e-commerce performance across orders, deliveries, product categories, customer behavior, and seller efficiency. Using SQL, Python, and visualization tools, it uncovers key insights on sales patterns, delivery performance, customer segmentation, product affinity, and lead conversion—helping identify growth opportunities, improve logistics, and enhance overall business strategy.

## Business Problem Statement :

1. Order Management Inefficiency: Identify delays or irregularities in order processing and fulfillment affecting customer satisfaction.

2. Delivery Optimization: Analyze delivery times and logistics performance to minimize late deliveries and improve operational efficiency.

3. Product Performance Gaps: Evaluate sales trends and product category demand to optimize inventory and marketing strategies.

4. Sales Prediction Accuracy: Develop data-driven models to forecast future sales and support better business planning.

5. Customer Sentiment Analysis: Assess order reviews to understand satisfaction levels and detect service or product issues.

6. Customer Segmentation: Cluster customers based on behavior and purchase patterns to enable targeted marketing.

7. Customer Lifetime Value (CLV): Measure long-term profitability per customer to prioritize high-value segments.

8. Product Affinity Insights: Identify frequently bought-together products to enhance cross-selling and bundling strategies.

9. Seller Performance Evaluation: Assess sellers based on review scores, sales, and delivery times to improve marketplace quality.

10. Lead Conversion Optimization: Analyze marketing channel effectiveness to boost conversion rates and reduce acquisition costs.


## Dataset Overview :

The project uses a publicly available E-commerce dataset (Olist – Kaggle) containing over 100K orders (2016–2018).
It includes data on orders, customers, products, sellers, payments, and reviews, enabling analysis of sales trends, customer behavior, and business performance across multiple dimensions.

## Tools & Techniques :

Tools: Python, Power BI, SQL, Excel

 Techniques: Data Cleaning, Exploratory Data Analysis (EDA),  Customer Segmentation, Sales Forecasting, Product Affinity Analysis, and Data Visualization

## Table Structure :

Olist_Ecommerce_Analytics/
│
├── data/
│   ├── olist_orders_dataset.csv
│   ├── olist_products_dataset.csv
│   ├── olist_customers_dataset.csv
│   ├── olist_sellers_dataset.csv
│   ├── olist_order_reviews_dataset.csv
│   └── olist_order_payments_dataset.csv
│
├── notebooks/
│   └── Olist_Ecommerce_Analytics.ipynb
│
├── dashboards/
│   ├── Sales_Revenue_Insights.png
│   ├──Customer_Seller_Insights.png │
│   ├──Order_Delivery_Insights.png
│
├── README.md
└── requirements.txt

## 🧹 Data Cleaning & Preparation

1. **Imported datasets** from multiple CSV files — orders, products, customers, sellers, reviews, and payments.


2. **Checked** for missing values and handled them using mean, mode, or removal where necessary.

3. **Removed duplicates** across order and customer datasets to ensure data accuracy.

4. **Standardized column** names for consistency (e.g., order_id, customer_id, product_category_name).

5. **Converted data types** — date columns to datetime, numerical columns to float/int.

6. **Created** new derived columns such as delivery duration and total order value.

7. **Merged datasets** using unique identifiers (order_id, customer_id, seller_id) for unified analysis.

8. **Filtered** out invalid or incomplete transactions (e.g., canceled or unreviewed orders).

9. **Encoded categorical variables** (like product category) for analytics and modeling.

10. **Scaled numerical features** before predictive analysis to maintain uniformity.

## 📊 Exploratory Data Analysis (EDA) Insights

### Order Trends :

**.** Total of 99K+ orders analyzed across Brazil.

**.** Majority of orders fall between 2017–2018, showing Olist’s   rapid growth phase.

**.** Highest sales months: November and December — indicating  strong festive season demand.

<img width="1193" height="523" alt="Screenshot 2025-11-03 131402" src="https://github.com/user-attachments/assets/a7dcb1e5-d8e9-49e0-a7b6-0a57663bfead" />


### Order Delivery Insights :

**.** 65% orders delivered on time, while 35% faced delays due to logistics or regional issues.

**.** Average delivery time: ~12 days; fastest deliveries observed in Southeast Brazil.

**.** Late deliveries highly correlated with long-distance shipments.

<img width="1689" height="803" alt="Screenshot 2025-11-03 174134" src="https://github.com/user-attachments/assets/33be747e-37e5-4cf6-9221-0536dc5dc7ff" />


### Product Categories :

**.** Top categories: Health & Beauty, Watches, and Computers.

**.** Electronics and Furniture contribute the highest revenue share.

**.** Niche segments (e.g., Automotive Accessories, Fashion) show potential for growth.

<img width="1697" height="899" alt="Screenshot 2025-11-03 173947" src="https://github.com/user-attachments/assets/a6270509-6b88-4c5d-bfcb-c1758d831a37" />


### Sales Prediction Insights :

**.** Seasonal peaks and promotional periods boost sales volumes significantly.

**.** Predictive model shows 85–90% accuracy in forecasting sales trends.

**.** Key sales drivers: product category, delivery time, and customer region.

### Customer Segmentation:

**.** Customers segmented into Loyal, Occasional, and New Buyers using RFM analysis.

**.** Loyal customers (20%) contribute nearly 60% of total revenue.

**.** New customers show higher return and delay complaint rates.

### Customer Lifetime Value (CLV) :


**.** Average CLV: ~R$ 450.

**.** High-value customers mostly purchase electronics, home goods, and beauty products.

**.** Retention-focused offers could increase CLV by 15–20%.

### Product Affinity :


**.** Strong association between electronics & accessories, and beauty & health items.

**.** Cross-selling these products could raise overall basket value.

### Sellers Performance :


**.** Top 10% of sellers contribute ~60% of sales.

**.** Sellers with consistent delivery speed and good ratings retain more repeat customers.

**.** Some sellers show high cancellation or delayed shipment rates.

## Lead Conversion :


**.** Conversion rate: ~25%.

**.** Faster responses and positive reviews significantly improve conversion.

**.** High-value leads often come from repeat buyers and referral-based traffic.

### Order Reviews :


**.** Average rating: 4.1/5.

**.** Negative reviews mainly relate to delays or damaged products.

**.** Improving packaging and logistics can enhance satisfaction metrics.

### 📈 Key Findings :

**Delivery Performance**: 65% of orders are delivered on time; delays mainly occur due to longer distances and regional logistics inefficiencies.

**Product Insights:** Electronics, Beauty, and Home products dominate both in sales and customer engagement.

**Sales Forecasting:** Predictive models achieved ~90% accuracy; strong seasonal peaks observed during November–December.

**Customer Segmentation:** Loyal customers (20%) contribute 60% of total revenue — retention strategies here can yield high ROI.

**CLV Analysis:** Average CLV stands at R$450; offering personalized discounts could raise CLV by up to 20%.

**Product Affinity:** Cross-selling electronics with accessories and pairing beauty items boosts overall order value.

**Seller Insights:** Top 10% sellers generate 60% of sales; consistent service quality is key to positive ratings.

**Lead Conversion:** Conversion rate is 25%; faster communication and reviews strongly impact conversion success.

**Customer Feedback:** Overall satisfaction is good (avg rating 4.1/5); main issues involve delivery delays and damaged products.

### 📊 About the Dashboard : 

The Olist E-commerce Analytics Project consists of three interactive Power BI dashboards designed to analyze customer behavior, sales performance, and delivery operations. These dashboards provide comprehensive business insights across different dimensions such as geography, product category, payment methods, and order status.

#### 1️⃣ Sales & Revenue Overview Dashboard

**.** Displays total sales (13.59M), total orders (99K), and total product categories (73).

**.** Identifies top-selling product categories and top 5 cities by sales.

**.** Shows payment type distribution, revealing that credit cards dominate with ~78% of payments.

**.** Tracks average delivery time by city/state, highlighting regional performance variations.

<img width="1327" height="755" alt="Screenshot 2025-11-03 173244" src="https://github.com/user-attachments/assets/fdd46170-22d1-47aa-ae67-a48bcb350b54" />


#### 2️⃣ Customer & Seller Insights Dashboard

**.** Highlights total customers (99K), total revenue (15.84M), and average review rating (4 stars).

**.** Analyzes customer segmentation by city and top-spending customers.

**.** Visualizes customer distribution on a map, aiding geographic targeting and marketing strategy.

<img width="1335" height="749" alt="Screenshot 2025-11-03 173258" src="https://github.com/user-attachments/assets/287ed3f8-5dbe-4bba-955a-eb013dda430e" />


#### 3️⃣ Order & Delivery Insights Dashboard

**.** Evaluates freight costs, delivery performance, and order status by category.

**.** Compares product dimensions (height, length, weight) with revenue.

**.** Displays seller concentration across states and average freight values.

**.** Highlights top-performing categories by revenue, such as beleza_saude and relogios_presentes.

<img width="1074" height="617" alt="Screenshot 2025-11-03 173330" src="https://github.com/user-attachments/assets/a813fe97-3d88-4745-ad48-10e07c1963e7" />


## Final Recommendations :

***.*** Optimize delivery routes to reduce delays.

***.*** Focus on high-selling categories for revenue growth.

***.***  Implement loyalty programs for repeat customers.

***.***  Promote diverse payment options to boost sales.

***.***  Support low-performing sellers through training.

***.*** Optimize product size and freight costs.

***.*** Use customer segmentation for targeted marketing.

### Author & Content :

Kratika Gupta

Aspiring Data Analytics

*Email:* kratikagupta0517@gmail.com

*LinkedIn:*   www.linkedin.com/in/kratika-gupta-88309828a
