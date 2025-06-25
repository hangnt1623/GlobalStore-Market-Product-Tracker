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
- Prioritize Investment: APAC (high revenue, good margin, high retention), EU (highest profit, reduce returns), and Africa (near 0% returns, high potential)
- Review & Reassess: Canada (high margin but 93% churn), LATAM (low profit/revenue, high risk), and US (large scale, but retention/returns suboptimal).

**2. Strategic Products**
- Technology (Accessories & Phones): Expand portfolio, boost marketing, control costs.
- Office Supplies: Maintain stability, no large-scale expansion needed; focus on high-profit groups.
- Furniture: Restructure (cut/adjust weak groups); stop expansion if no improvement.

**3. Customer Segments (Bonus)**
- Corporate: Prioritize retention (high profit, stable purchases)
- Consumer: Improve shopping experience (high return rate)
- Home Office: Explore upsell strategies (good retention, low revenue)

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

1️⃣ Empathize  

(1) 5W1H 

<img width="769" alt="{D7F1D2E4-C029-4F20-A585-07632938B605}" src="https://github.com/user-attachments/assets/4f2f7807-0821-4c6a-aa86-932f576750d5" />

(2) Empathy Map

<img width="550" alt="{8C24B7EC-F3DB-4B3E-AD70-F8580E23482B}" src="https://github.com/user-attachments/assets/f3af8ac1-fb2d-4abc-87a3-35b41bc7e30f" />

(3) Stakeholder need

<img width="275" alt="{D50B829C-E92C-4DEB-BD63-1D3AA8FEF8A0}" src="https://github.com/user-attachments/assets/15065acb-0f3f-468f-b8ef-dd8b4c8de902" />

2️⃣ Define point of view  

(1) North Star Metric

<img width="474" alt="{7C0B8BA0-4E66-4B5D-A2D4-C1B861934E3F}" src="https://github.com/user-attachments/assets/6bc1c95c-8746-49fc-bd04-92350d99ae18" />

(2) Point of view 

<img width="555" alt="{5085A3E8-8C89-4603-BEAE-5D5D1EB893AD}" src="https://github.com/user-attachments/assets/13d315e1-97ce-4923-b088-f2cd36f6a6c6" />


3️⃣ Ideate  

<img width="882" alt="{010387AB-97F1-4BDE-8762-A52A614D1685}" src="https://github.com/user-attachments/assets/87d052be-c103-4253-b3a5-d16548acc40f" />



4️⃣ Prototype and review  

This part is presented in Dashboard.

## ⚒️ Main Process

1️⃣ Data Cleaning & Preprocessing  
2️⃣ Exploratory Data Analysis (EDA)  
3️⃣ Power BI Visualization  
---

## 📊 Key Insights & Visualizations  

### 🔍 Dashboard Preview & Analysis

#### 1️⃣ Dashboard 1: Overview

<img width="740" alt="{E843165D-44C6-4C7E-941B-35FDE78B5809}" src="https://github.com/user-attachments/assets/a6d8dd17-6a38-49ca-bfb7-c99d98cdeb97" />

**📌 Analysis 1**

***Oberservations***
- Profitability (North Star Metric): Overall Profit Margin is 11.61%, showing stability over time, despite fluctuations. Sales and Profit grow in parallel (Sales YOY: 51.55%).
- Customer Health: High Retention Rate (92.23%) and low Churn Rate (7.77%) indicate strong customer loyalty.
- Category Profit Disparity: Technology and Office Supplies show strong Profit Margins (both ~14%), significantly outperforming Furniture (only 7% Profit Margin).
- Segment Profit Uniformity: All customer segments (Home Office, Corporate, Consumer) exhibit similar Profit Margins (~12%). However, Corporate has the highest Return Rate compared to Home Office and Consumer.

***Recommendations***
- Enhance Furniture Profitability: Deep dive into the 7% Profit Margin of Furniture to identify cost or pricing issues. This is crucial for improving the overall Profit Margin.
- Capitalize on Top Categories: Continue investing in Technology and Office Supplies to leverage their strong (~14%) Profit Margins.
- Address Corporate Returns: Investigate the high Return Rate in the Corporate segment to protect its ~12% Profit Margin.
- Sustain Overall Growth: Maintain strategies driving strong sales growth (51.55% YOY) and high retention to support the stable 11.61% Profit Margin.

#### 2️⃣ Dashboard 2: Market Tracker
<img width="744" alt="{B71DE64E-B43A-4DB4-B3A9-6D5887CA3814}" src="https://github.com/user-attachments/assets/73ef3283-2ba2-44aa-ab09-ea95603a863a" />

**📌 Analysis 2**

***Oberservations***
- Strong & Stable Markets:
   + APAC: Largest sales share (28.36%), healthy 12.16% Profit Margin, and good 84.91% Retention
   + EU: High sales share (23.24%), highest Profit Margin (12.69%), but also the highest Return Rate (6.21%)
   + US: Significant sales share (18.17%), strong 12.47% Profit Margin, but moderate 5.95% Return Rate
- Promising Market with Challenges:
   + Africa: Good 11.34% Profit Margin with exceptionally low 0.04% Return Rate, but suffers from very low 53.21% Retention and high 46.79% Churn
- Markets Needing Urgent Review:
  + LATAM: Moderate 10.24% Profit Margin and moderate Return Rate (5.82%)
  + EMEA: Lowest Profit Margin (5.45%) and very high 40.85% Churn Rate
  + Canada: Exceptionally high 26.62% Profit Margin, but critically unsustainable with 93.44% Churn Rate and minimal sales share (0.53%)

***Recommendations***
- Sustain & Optimize Strong Markets
  + APAC: Continue investment to leverage scale and 12.16% PM
  + EU: Prioritize reducing its 6.21% Return Rate to maximize the 12.69% PM
  + US: Focus on improving retention and reducing its 5.95% Return Rate to solidify 12.47% PM.
- Develop Africa's Retention: Invest in strategies to boost retention and reduce churn in Africa, capitalizing on its good 11.34% PM and minimal returns
- Strategic Review for Challenging Markets:
  + LATAM: Optimize operations and address its 5.82% Return Rate to enhance its 10.24% PM
  + EMEA: Requires a major strategic overhaul to address the 5.45% PM and very high churn
  + Canada: Investigate the extreme churn (93.44%) despite high 26.62% PM; unsustainable for growth


#### 3️⃣ Dashboard 3 Preview  
<img width="735" alt="{0A5C27CE-4293-4B59-9103-9B1DAFFF741E}" src="https://github.com/user-attachments/assets/77e35abe-adf9-4909-89b6-0faedee1c865" />

**📌 Analysis 3**

***Oberservations***
- Product Category Performance:
  + Technology (37.53% sales) & Furniture (32.51% sales) are top revenue, but Technology has Profit Margin increase gradually between 13~14%
  + Office Supplies (29.96% sales) shows consistently low and declining Profit Margin (~3-5%), significantly impacting overall PM
- Customer Segment Health by Category:
  + Office Supplies has the highest Retention Rate (~89.32%)
  + Furniture has the highest Return Rate (~6-7.5%) and the lowest Profit Margin, with sub-categories even showing negative PM
- Sub-Category Profitability:
  + High PM: Paper (24.24%), Labels (20.45%), Envelopes (17.32%), Copiers (17.13%) (Office Supplies); Accessories (17.30%) (Technology)
  + Low/Negative PM: Tables (-8.46%), Chairs (9.35%) (Furniture); Machines (7.56%) (Technology); Storage (9.62%), Supplies (9.29%) (Office Supplies)

***Recommendations***
- Maximize Technology: Invest in Technology to capitalize on its increasing 13-14% PM
- Urgent Office Supplies Review: Investigate reasons for Office Supplies' declining ~3-5% PM despite high retention; focus on high-PM sub-categories
- Restructure Furniture: Address high returns and eliminate/re-evaluate loss-making Furniture (e.g., Tables: -8.46% PM)
- Optimize Sub-Categories: Promote high-PM items (Paper, Labels) and improve/review low-PM items (Machines, Storage, Supplies)


---

## 🔎 Final Conclusion & Recommendations  

👉🏻 Based on the insights and findings above, we would recommend the [stakeholder team] to consider the following:  

📌 Key Takeaways:  
✔️ Recommendation 1  
✔️ Recommendation 2  
✔️ Recommendation 3
