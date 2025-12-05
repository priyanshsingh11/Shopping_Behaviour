# 📊 Customer Shopping Behavior Analysis  
### A Complete Data Analytics & BI Project (Python + SQL + Power BI)

This project analyzes **3,900 customer shopping transactions** to uncover insights about purchase behavior, product preferences, customer segments, and revenue patterns.

The workflow combines **Python (EDA & Cleaning)**, **PostgreSQL (Business Queries)**, and **Power BI (Dashboard Development)** to deliver a full end-to-end analytics solution.

---

## 🔗 Project Links  
- **Power BI Dashboard:** https://app.powerbi.com/groups/53a5befb-1a9b-4280-a68d-314129fa1ccc/reports/a3fc865d-37c6-4a9e-9194-35a15903f1a5?ctid=cb1013ae-fb33-4405-8464-8d4ebfd3679d&pbi_source=linkShare  
- **PDF Report:** Included in the repository  

---

## 📁 Dataset Summary  

Based on the project documentation:

- **Rows:** 3,900  
- **Columns:** 18  
- **Key features include:**  
  - Customer demographics (Age, Gender, Location, Subscription Status)  
  - Purchase details (Item, Category, Amount, Size, Color, Season)  
  - Behavioral attributes (Discount Applied, Promo Code, Previous Purchases, Rating, Shipping Type)  
- **Missing Values:**  
  - 37 missing values in **Review Rating**  

---

## 🧹 Data Preparation & Cleaning (Python)

Performed using **pandas**, **matplotlib**, and **seaborn**.

### ✔ Data Loading & Exploration  
- Used `df.info()` and `df.describe()` for structure and summary.  
- Identified missing values and inconsistent fields.

### ✔ Handling Missing Data  
- Missing Review Ratings were imputed using **median rating per product category**.

### ✔ Column Standardization  
- All column names were converted to **snake_case** for consistency.

### ✔ Feature Engineering  
- `age_group` → created by binning age values  
- `purchase_frequency_days` → derived using previous purchase timestamps  

### ✔ Data Consistency  
- Verified overlap between **discount_applied** and **promo_code_used**.  
- Dropped redundant **promo_code_used** column.

### ✔ Database Integration  
- Cleaned dataset loaded into **PostgreSQL** for structured SQL analysis.

---

## 🧾 Business Analysis Using SQL (PostgreSQL)

The PDF (pages 2–6) includes insights such as:

### 1️⃣ Revenue by Gender  
Comparison of total spending by male vs female customers.

### 2️⃣ High-Spending Discount Users  
Customers who used discounts but still spent above-average amounts.

### 3️⃣ Top 5 Products by Rating  
Products like **Gloves**, **Sandals**, and **Boots** ranked highest (page 4).

### 4️⃣ Shipping Type Comparison  
**Express shipping** users spent more than standard shipping users (page 4).

### 5️⃣ Subscribers vs Non-Subscribers  
Insights into:  
- Avg spend  
- Total customers  
- Revenue contribution (page 4)

### 6️⃣ Discount-Dependent Products  
Ranked products by how often discounts were used.

### 7️⃣ Customer Segmentation  
Based on purchase frequency:  
- New  
- Returning  
- Loyal

### 8️⃣ Top 3 Products Per Category  
Clothing, Accessories, Footwear, etc. (page 6)

### 9️⃣ Repeat Buyers & Subscriptions  
Correlation between **>5 purchases** and subscription likelihood.

### 🔟 Revenue by Age Group  
Young Adults contributed the highest revenue (page 7).

---

## 📊 Power BI Dashboard

The interactive dashboard (page 7) includes:

- Total Customers  
- Average Purchase Amount  
- Average Review Rating  
- Revenue by Category  
- Subscription Status Distribution  
- Revenue by Age Group  
- Sales by Category  

**Filters:** Gender, Category, Shipping Type, Subscription, Season  

This dashboard enables stakeholders to quickly interpret trends and identify growth opportunities.

---

## 💡 Business Recommendations  

Based on insights (page 8):

### 🔹 Boost Subscriptions  
Offer exclusive deals and discounts.

### 🔹 Strengthen Loyalty Programs  
Reward Returning customers to convert them into Loyal ones.

### 🔹 Optimize Discount Strategy  
Balance discount usage with profit margins.

### 🔹 Improve Product Positioning  
Promote top-rated and best-selling items.

### 🔹 Targeted Marketing  
Focus on:  
- High-revenue age groups  
- Express-shipping customers  
- Popular categories  

---

## 🛠 Tech Stack

- **Python** → EDA, cleaning, feature engineering  
- **PostgreSQL** → Business logic & SQL analysis  
- **Power BI** → Visualization & Dashboard  
- **Pandas, NumPy** → Data manipulation  
- **Matplotlib, Seaborn** → Charts & exploration  

---

## 📂 Recommended Folder Structure

/Customer-Shopping-Behavior-Analysis
│
├── data/
│ └── customer_data.csv
│
├── notebooks/
│ └── eda_and_cleaning.ipynb
│
├── sql/
│ └── business_queries.sql
│
├── dashboard/
│ └── Customer Behavior Dashboard.pbix
│
├── reports/
│ └── Customer Shopping Behavior Analysis.pdf
│
└── README.md


---

## 🚀 How to Run the Project

### 1. Clone the repository  
git clone https://github.com/yourusername/CustomerShoppingAnalysis.git
cd CustomerShoppingAnalysis

shell
Copy code

### 2. Install required Python libraries  
pip install -r requirements.txt

yaml
Copy code

### 3. Run the Python notebook  
Open the Jupyter Notebook in `/notebooks` to clean and preprocess the data.

### 4. Import cleaned data into PostgreSQL  
Execute the SQL queries provided in `/sql`.

### 5. Open the Power BI dashboard  
Load the `.pbix` file from `/dashboard` and refresh connections.

---

## 🎉 Final Notes  
This project showcases complete analytics lifecycle skills:  
**Data Cleaning → EDA → SQL Insights → BI Dashboard → Business Recommendations.**

Feel free to explore, modify, or extend the analysis!
