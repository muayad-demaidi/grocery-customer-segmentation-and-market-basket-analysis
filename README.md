🛒 Grocery Customer Segmentation & Market Basket Analysis
📌 Project Overview

This project analyzes 38,000+ grocery transactions to uncover customer behavior patterns, segment customers based on visit frequency, and identify frequently purchased product combinations.

The goal is to transform raw transaction data into actionable retail insights that can support marketing strategy, inventory planning, and cross-selling optimization.

📊 Dataset

Source: Public grocery transaction dataset

Records after cleaning: 38,006 transactions

Key columns:

Member_number

Date

itemDescription

🧹 Data Preparation

Removed duplicate records (759 rows)

Verified no missing values

Converted Date column to datetime

Extracted:

DayOfWeek

Month

Created transaction-level basket structure for association rule mining

👥 Customer Behavior Analysis
📈 Visit Frequency

Average visit interval: 45.7 days

Median visit interval: 41 days

Significant variation across customers

This indicates mostly monthly purchasing behavior with a subset of infrequent (seasonal) shoppers.

🏆 Top Selling Products
Rank	Product	Sales
1	whole milk	2363
2	other vegetables	1827
3	rolls/buns	1646

Staple products dominate recurring traffic.

🧠 Customer Segmentation
Methodology

Features used:

Average days between visits

Favorite shopping day

One-hot encoding applied to weekday

Features standardized

Optimal number of clusters selected using Silhouette Score

Algorithm used: K-Means

Result

Identified 8 customer segments, mostly differentiated by:

Visit cycle (~40–45 days for most segments)

Preferred shopping weekday

This enables targeted weekday promotions and behavioral marketing strategies.

🛍 Market Basket Analysis
Approach

Grouped transactions by customer and date

Applied One-Hot Encoding

Used Apriori Algorithm

Minimum support: 0.005

Association metric: Lift > 1.0

Key Product Associations

frankfurter → other vegetables (Lift = 1.11)

yogurt → sausage (Lift = 1.10)

soda → sausage (Lift = 1.01)

These associations suggest product bundling and optimized shelf placement opportunities.

💼 Business Insights

📅 Day-based promotional campaigns

🛒 Product bundling to increase basket size

📦 Inventory optimization based on seasonal demand

🤖 Foundation for recommendation systems

🧰 Tools & Technologies

Python

Pandas

Matplotlib & Seaborn

Scikit-learn (K-Means, Silhouette Score)

mlxtend (Apriori & Association Rules)

🚀 Key Skills Demonstrated

Data cleaning & preprocessing

Feature engineering

Exploratory data analysis (EDA)

Customer segmentation

Association rule mining

Translating analytics into business strategy

If you found this project interesting or would like to collaborate, feel free to connect.
