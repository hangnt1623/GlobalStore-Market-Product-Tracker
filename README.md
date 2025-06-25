# 📊 PowerBI_Market Expansion & Product Strategy

- Author: Nguyen Thuy Hang
- Date: 2025-06-23
- Tools Used: Power BI

---

## 📑 Table of Contents  
1. [📌 Background & Overview](#-background--overview)  
2. [📂 Dataset Description & Data Structure](#-dataset-description--data-structure)  
3. [🧠 Design Thinking Process](#-design-thinking-process)  
4. [📊 Key Insights & Visualizations](#-key-insights--visualizations)  
5. [🔎 Final Conclusion & Recommendations](#-final-conclusion--recommendations)

---

## 📌 Background & Overview  

### Objective:
### 📖 What is this project about? 
 
- Provide a brief introduction to the project. Define the problem statement and why it is important.
- Write in bullet point format

 _Example:_
 
 This project analyzes sales trends and inventory control using SQL and Power BI. The objective is
 - optimize stock levels & improve demand forecasting
 - reduce costs.  

### 👤 Who is this project for?  

Mention who might benefit from this project 

 _Example:_

✔️ Data analysts & business analysts  
✔️ Supply chain managers & inventory controllers  
✔️ Decision-makers & stakeholders  

###  ❓Business Questions:  
Clearly outline what the business questions project will solve.  

 _Example:_

✔️ Identify high-demand products and sales trends.  
✔️ Optimize inventory levels to prevent overstocking or stockouts.  
✔️ Provide actionable insights through Power BI dashboards.  

### 🎯Project Outcome:  
Summarize key findings and insights/ trends/ themes in a concise, bullet-point 
format.  

 _Example:_

✔️ Sales Trends: The top X% of products generate Y% of revenue.  
✔️ Inventory Optimization: Certain products are frequently out-of-stock, causing revenue loss.  
✔️ Customer Behavior: Returning customers spend Z% more per transaction than new customers.  

---

## 📂 Dataset Description & Data Structure  

### 📌 Data Source  
- Source: The dataset is obtained from—Kaggle.
- Size:
  + The Orders table contains 51,290 records
  + The People table contains 13 records
  + The Returns table contains 1,172 records
- Format: .csv

### 📊 Data Structure & Relationships  

#### 1️⃣ Tables Used:  
There are 3 tables in the dataset:
- Orders: store transaction information
- People: store information of sellers in each area
- Returns: record returned transactions

#### 2️⃣ Table Schema & Data Snapshot  

#### 3️⃣ Data Relationships
<img width="509" alt="{6E33EAAF-1C3E-418A-AF83-FB59D06A0EF6}" src="https://github.com/user-attachments/assets/bf300ab1-2b72-4985-b89f-b8855dc01cc6" />
 
 (1) dim_Date to Orders:
- Connection Type: One-to-many (1:*)
- Direction: Single direction (from dim_Date to Orders)
- Description: For each unique Date in the dim_Date table, there can be multiple corresponding Order Date entries in the Orders table.  This allows for filtering and analyzing orders based on time dimensions.

(2) dim_Subcategory to Orders:
- Connection Type: One-to-many (1:*)
- Direction: Single direction (from dim_Subcategory to Orders)
- Description: Each Sub-Category in the dim_Subcategory table can be associated with multiple orders in the Orders table. This is used to categorize and analyze orders by subcategory

(3) dim_Segment to Orders:
- Connection Type: One-to-many (1:*)
- Direction: Single direction (from dim_Segment to Orders)
- Description: A single Segment can be linked to multiple orders in the Orders table. This allows for analysis of orders based on customer segments

(4) dim_Market to Orders:
- Connection Type: One-to-many (1:*)
- Direction: Single direction (from dim_Market to Orders)
- Description: Each Market can have multiple associated orders. This is used to analyze order performance across different markets

(5) People to Orders:
- Connection Type: One-to-many (1:*)
- Direction: Single direction (from People to Orders)
- Description: Each Person in the People table (likely representing a salesperson or responsible party for a region) can be associated with multiple orders. This enables performance tracking by individual or region

(6) Orders to Returns:
- Connection Type: One-to-many (1:*)
- Direction: Single direction (from Orders to Returns)
- Description: An Order ID in the Orders table can have zero or one corresponding Order ID in the Returns table (if the order was returned)

---

## 🧠 Design Thinking Process  

Explain the step-by-step approach taken to solve the problem.  

👉🏻 Insert a screenshot of the Design Thinking steps (Screenshot your Excel design thinking tables for better presentation).  

1️⃣ Empathize  
2️⃣ Define point of view  
3️⃣ Ideate  
4️⃣ Prototype and review  

---

## ⚒️ Main Process

1️⃣ Data Cleaning & Preprocessing  
2️⃣ Exploratory Data Analysis (EDA)  
3️⃣ SQL/ Python Analysis 

- In each step, show your Code

- Include query/ code execution screenshots or result samples

- Explain its purpose and its findings


4️⃣ Power BI Visualization  (applicable for PBI Projects)

---

## 📊 Key Insights & Visualizations  

### 🔍 Dashboard Preview  

#### 1️⃣ Dashboard 1 Preview  
👉🏻 Insert Power BI dashboard screenshots here  

📌 Analysis 1:  
- Observation: _Describe trends, key metrics, and patterns._  
- Recommendation: _Suggest actions based on insights._  

#### 2️⃣ Dashboard 2 Preview  
👉🏻 Insert Power BI dashboard screenshots here

📌 Analysis 2:   
- Observation: _Describe trends, key metrics, and patterns._  
- Recommendation: _Suggest actions based on insights._  

#### 3️⃣ Dashboard 3 Preview  
👉🏻 Insert Power BI dashboard screenshots here  

📌 Analysis 3:  
- Observation: _Describe trends, key metrics, and patterns._  
- Recommendation: _Suggest actions based on insights._  

---

## 🔎 Final Conclusion & Recommendations  

👉🏻 Based on the insights and findings above, we would recommend the [stakeholder team] to consider the following:  

📌 Key Takeaways:  
✔️ Recommendation 1  
✔️ Recommendation 2  
✔️ Recommendation 3
