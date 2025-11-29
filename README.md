📊 Customer Shopping Behavior Analysis
A Complete Data Analytics & BI Project (Python + SQL + Power BI)
📌 Project Overview

This project analyzes 3,900 customer shopping transactions to uncover actionable insights about purchase behavior, product preferences, customer segments, and revenue patterns.
The workflow integrates Python (EDA & Cleaning), PostgreSQL (Business Queries), and Power BI (Dashboard Development) to deliver a full end-to-end analytics solution.

Power BI Dashboard Link: (add your shortened link here)
PDF Report: Included in repository

📁 Dataset Summary

Based on the project documentation 

Customer Shopping Behavior Anal…

:

Rows: 3,900

Columns: 18

Key features include:

Customer demographics (Age, Gender, Location, Subscription Status)

Purchase details (Item, Category, Amount, Size, Color, Season)

Behavior features (Discount Applied, Promo Code, Previous Purchases, Frequency, Rating, Shipping Type)

Missing values:

37 missing values in Review Rating column

🧹 Data Preparation & Cleaning (Python)

Performed in Python using pandas, matplotlib, and seaborn:

✔ Data Loading & Exploration

Used df.info(), df.describe() to understand structure and distributions.

✔ Handling Missing Data

Missing Review Rating values were imputed using median rating per product category.

✔ Column Standardization

Converted all column names to snake_case for clarity and consistency.

✔ Feature Engineering

age_group → created by binning age values

purchase_frequency_days → derived using previous purchase timestamps

✔ Data Consistency & Redundancy

Verified overlap between discount_applied & promo_code_used; later dropped promo_code_used.

✔ Database Integration

Loaded cleaned dataset into PostgreSQL for structured business analysis.

🧾 Business Analysis Using SQL (PostgreSQL)

Key SQL insights extracted in the analysis (documented in PDF pages 2–6) 

Customer Shopping Behavior Anal…

:

1️⃣ Revenue by Gender

Compared total revenue from male vs female customers.

2️⃣ High-Spending Discount Users

Identified customers using discounts but still spending above average purchase value.

3️⃣ Top 5 Products by Rating

Products with highest average review rating (e.g., Gloves, Sandals, Boots — page 4).

4️⃣ Shipping Type Comparison

Express shipping users spend more on average than Standard shipping users (page 4).

5️⃣ Subscribers vs Non-Subscribers

Comparison of:

Total customers

Average spend

Total revenue
(Example: Subscribers generated significant revenue — page 4)

6️⃣ Discount-Dependent Products

Ranked products based on % of discounted purchases.

7️⃣ Customer Segmentation

Used purchase frequency to classify customers as:

New

Returning

Loyal

8️⃣ Top 3 Products per Category

Displayed top-selling items under Clothing, Accessories, Footwear, etc. (page 6)

9️⃣ Repeat Buyers & Subscriptions

Analyzed correlation between >5 purchases and subscription likelihood.

🔟 Revenue by Age Group

Young Adults contributed the highest revenue (page 7).

📊 Power BI Dashboard

An interactive Customer Behavior Dashboard was built to visualize insights (page 7):
Features include:

Total Customers

Average Purchase Amount

Average Review Rating

Revenue by Category

Subscription Status Distribution

Revenue by Age Group

Sales by Category

Filters: Gender, Category, Shipping Type, Subscription, Season

This dashboard allows stakeholders to quickly interpret trends and identify opportunities for growth.

💡 Business Recommendations

Based on insights (summarized from page 8) 

Customer Shopping Behavior Anal…

:

🔹 Boost Subscriptions

Offer benefits and exclusive deals to increase conversions.

🔹 Strengthen Customer Loyalty Programs

Reward repeat buyers to move them from Returning to Loyal.

🔹 Optimize Discount Strategy

Balance sales growth with margin preservation.

🔹 Improve Product Positioning

Promote top-rated and best-selling products to enhance sales.

🔹 Targeted Marketing

Focus on:

High-revenue age groups

Express-shipping customers

Popular product categories

🛠 Tech Stack

Python → Data cleaning, EDA, feature engineering

PostgreSQL → Business logic & SQL analytics

Power BI → Dashboard & Interactive visualization

Pandas, NumPy → Data manipulation

Matplotlib/Seaborn → Exploratory charts

📂 Folder Structure (Recommended)
/Customer-Shopping-Behavior-Analysis
│
├── data/
│   └── customer_data.csv
│
├── notebooks/
│   └── eda_and_cleaning.ipynb
│
├── sql/
│   └── business_queries.sql
│
├── dashboard/
│   └── Customer Behavior Dashboard.pbix
│
├── reports/
│   └── Customer Shopping Behavior Analysis.pdf
│
└── README.md

🚀 How to Run the Project
1. Clone the repository
git clone https://github.com/yourusername/CustomerShoppingAnalysis.git
cd CustomerShoppingAnalysis

2. Install required Python libraries
pip install -r requirements.txt

3. Run the Python notebook

Clean and preprocess data using the Jupyter Notebook in /notebooks.

4. Import data into PostgreSQL

Use SQL scripts in /sql.

5. Open the Power BI dashboard

Load the .pbix file from /dashboard and refresh data sources.
