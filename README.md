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
This project analyzes global sales performance of Superstore using provided datasets (Orders, People, Returns). The objective is to:
- Provide an overview of the company's business situation: This includes understanding overall sales trends, revenue, and profitability
- Support market expansion strategies: By identifying top-performing regions, untapped markets, and customer segments
- Inform strategic product selection: By analyzing product performance, identifying best-sellers, and understanding customer preferences

### 👤 Who is this project for?  

✔️ Senior Manager of Superstore (mainly)
✔️ Sales and Marketing Teams  
✔️ Product Development Teams 
✔️ Regional Managers
✔️ Business Analysts

###  ❓Business Questions:  
✔️ Understand overall business performance by analyzing sales, profit, and quantity trends over time and across different segments
✔️ Identify high-potential markets for expansion and areas requiring strategic intervention based on regional performance
✔️ Pinpoint strategic products by evaluating profitability, sales contribution, and return rates of various product categories and sub-categories
✔️ Provide actionable insights and recommendations through an interactive Power BI dashboard to support the Senior Manager's decision-making process

### 🎯Project Outcome:  
**1. Market Expansion**
* **Prioritize Investment:**
    * **APAC:** Top revenue, good profit margin, and high customer retention make it a **strategic market**
    * **EU:** Boasts the **highest profit margin**; efforts should focus on reducing return rates for further optimization
    * **Africa:** Shows **high potential** with almost zero returns and a solid profit margin, indicating readiness for increased investment
* **Review & Reassess:**
    * **Canada:** Despite a high profit margin, its **93% churn rate** makes current efficiency unsustainable
    * **LATAM:** Characterized by low profit and revenue, coupled with high risk (returns and churn), necessitating a **complete strategy re-evaluation**
    * **US:** While large-scale, its **suboptimal retention and high return rates** require improvements in after-sales and customer care

**2. Strategic Products**
* **Technology (Accessories & Phones):** This category is ripe for **expansion**. We should prioritize expanding the portfolio, boosting marketing efforts, and maintaining cost control to maximize its strong profit margins.
* **Office Supplies:** This stable category requires **no large-scale expansion**. The focus should be on optimizing operational efficiency and further exploiting its high-profit sub-groups.
* **Furniture:** Requires urgent **restructuring**. We need to re-evaluate and adjust weak groups (e.g., cutting or changing supply chains). If improvements aren't seen, expansion should halt, retaining only profitable groups to prevent dragging down overall performance.

**3. Customer Segments (Bonus)**
* **Corporate:** Given its **high profit margin and stable purchase frequency**, retaining these customers should be a top priority
* **Consumer:** The **high return rate** in this segment indicates a need to improve the overall shopping experience and product quality
* **Home Office:** With good retention but **low revenue**, there's potential to implement **upsell strategies** to increase average transaction value

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
