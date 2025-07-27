## ✅ KPMG Excel Project – Full Step-by-Step (Humanized + Pivot Format)

---

### 🧹 Task 1: Clean the Data

#### 🏠 Customer Address
- Remove duplicate rows
- Standardize `state` names (e.g., NSW, QLD)

#### 👤 Customer Demographics
- Fix gender column → only “Male” or “Female”
- Clean `default` column → remove symbols like @, #, etc.
- Replace “NA”, “-”, “n/a” with blanks
- Make sure `DOB` looks like a proper date

#### 💳 Transactions
- Format `transaction_date` column as Date
- Remove rows with missing `transaction_id`, `list_price`, etc.

#### 🆕 New Customers
- Use `PROPER()` to clean messy address formatting
- Fix gender (standardize)
- Fix spelling or weird values in `job_title`, `job_industry_category`

💾 Save as: `Task1_Data_Cleaning.xlsx`

---

### 👥 Task 2: Customer Segmentation

#### 💰 Segmentation by Wealth Segment
- Pivot Table:
  - Rows = `wealth_segment`
  - Values = Count of `customer_id`, Average of `tenure`

#### 🚻 Segmentation by Gender
- Pivot Table:
  - Rows = `gender`
  - Values = Count of `customer_id`, Average of `past_3_years_bike_related_purchases`

#### 🏢 Segmentation by Job Industry
- Pivot Table:
  - Rows = `job_industry_category`
  - Columns = `wealth_segment`
  - Values = Count of `customer_id`

💾 Save as: `Task2_Customer_Segmentation.xlsx`

---

### 📊 Task 3: Transaction Analysis

#### 📈 Sales Trend (Monthly)
- Add a new column → Extract `Month` from `transaction_date`
- Pivot Table:
  - Rows = `Month`
  - Values = Sum of `list_price`
- Insert Line Chart to visualize

#### 🏷️ Product Performance
- Pivot Table 1:
  - Rows = `brand`
  - Values = Sum of `list_price`
- Pivot Table 2:
  - Rows = `product_line`
  - Values = Sum of `list_price`, Average of `list_price`

#### 👑 Top 10 Customers
- Pivot Table:
  - Rows = `customer_id`
  - Values = Sum of `list_price`
  - Sort by value (descending), filter top 10
- Avg Purchases = Total transactions / Total unique customers

💾 Save as: `Task3_Transaction_Analysis.xlsx`

---

### 🔎 Task 4: New Customer Insights

#### 📊 New Customer Demographics
- Pivot Table:
  - Rows = `wealth_segment`
  - Columns = `job_industry_category`
  - Values = Count of `first_name`, Average of `past_3_years_bike_related_purchases`

#### 🗺️ Location Analysis
- Pivot Table:
  - Rows = `state`
  - Values = Count of `first_name`
- Compare using charts
- Analyze the relationship between:
  - `property_valuation` vs `wealth_segment`

#### 💸 Revenue Estimation
- Add new column:
- Sum `Estimated_Revenue` for total potential revenue

💾 Save as: `Task4_NewCustomer_Insights.xlsx`

---

### 💰 Task 5: Customer Lifetime Value (CLV)

#### 📏 Formula:

#### How to Calculate:
1. Merge `customer_demographic` with `transactions` on `customer_id`
2. For each customer:
   - Total Revenue = Sum of `list_price`
   - Purchase Count = Number of transactions
   - Tenure = from `customer_demographic`
   - APV = Revenue / Purchase Count
3. Purchase Frequency (PF) = Total transactions / Unique customers
4. CLV = (APV × PF) × Tenure

#### Segment CLV:
- Pivot Table 1:
  - Rows = `wealth_segment`
  - Values = Average of `CLV`
- Pivot Table 2:
  - Rows = `gender` or `job_industry_category`
  - Values = Average of `CLV`

💾 Save as: `Task5_CLV_Analysis.xlsx`

---

### 🧠 Task 6: Executive Summary

#### ✍️ Summary of Insights:
- Who are the top customers?
- Which job or gender group buys more?
- What brands or products sell best?
- Which states are full of high-potential new customers?

#### 💡 Recommendations:
- Focus on high-CLV customers and high-sales brands
- Target states with many high-value new customers
- Promote best-performing product lines

💾 Save as: `Task6_Executive_Summary.xlsx` or `.pptx`

---

### 🧳 Final Submission Checklist:
- [ ] All 6 Excel files ready
- [ ] Add your video link in any sheet
- [ ] Compress into `.zip` folder
- [ ] Upload on your dashboard

You're done ✅
