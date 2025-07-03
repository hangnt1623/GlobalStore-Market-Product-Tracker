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

#### 2️⃣ Data Relationships
<img width="685" alt="{1ECD2A48-763D-479B-A0F4-2CE4FFE14CEC}" src="https://github.com/user-attachments/assets/e1507170-410a-403f-9e63-4b1aba8410c1" />

---

## 🧠 Design Thinking Process  

Explain the step-by-step approach taken to solve the problem.  

1️⃣ Empathize  

(1) 5W1H 

<img width="685" alt="{CE7A0D03-D63F-4DE9-A25C-8C33F0AAE397}" src="https://github.com/user-attachments/assets/a3b3a7e5-27c4-4ec9-92b2-ea419f2006c3" />

<img width="685" alt="{8D425E12-81E5-4E4F-9BF5-F7C290C555C3}" src="https://github.com/user-attachments/assets/7e8fa7c0-0b93-4e6d-9d15-dd622f8d0a35" />


(2) Empathy Map

<img width="687" alt="{D87110DB-1A5F-40D3-B7A6-BB9755758910}" src="https://github.com/user-attachments/assets/1a621ac3-3aac-4e54-b913-bc031c8575b1" />

(3) Stakeholder need

<img width="685" alt="{54A28E57-1A7C-4D18-B8A0-3C02CC9DAE0B}" src="https://github.com/user-attachments/assets/cf9b985e-f85f-41dd-b7e1-7f792b331d9e" />


2️⃣ Define point of view  

(1) North Star Metric

<img width="689" alt="{2C521022-6453-4AB3-976F-194D09C3E5D4}" src="https://github.com/user-attachments/assets/a9194e90-059f-4439-af1b-61b93a1d36f5" />

(2) Point of view 

<img width="686" alt="{145BC1D8-98CA-41D3-89F2-5D6356703D75}" src="https://github.com/user-attachments/assets/5f0cdb09-34a7-4a54-99a2-6e385244eb8f" />


3️⃣ Ideate  

<img width="689" alt="{43661513-A425-4A30-8D55-B371D77A030B}" src="https://github.com/user-attachments/assets/f9971def-fc52-4088-a067-803a5e76e7ee" />

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


#### 3️⃣ Dashboard 3: Product Tracker
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

> **The company demonstrates strong growth and customer loyalty, yet the overall 11.61% Profit Margin is significantly weighed down by underperforming product categories and specific markets.**

👉🏻 Based on the insights and findings above, we would recommend Senior Manager to consider the following:  

📌 Market Recommendations
- Sustain Strong Markets: Keep investing in APAC, EU, and US. For EU and US, focus on reducing return rates to maximize profit
- Develop Africa's Potential: With good profit and low returns, prioritize improving retention and reducing churn to unlock growth
- Overhaul Challenging Markets:
  + EMEA: Major strategic overhaul needed due to very low Profit Margin (5.45%) and high churn
  + Canada: Investigate extreme churn (93.44%) despite high profit; it's unsustainable
  + LATAM: Optimize operations and address return rates

📌 Product Recommendations  
- Urgent Furniture Profitability Fix: The 7% Profit Margin and unprofitable Tables (-8.46% PM) are major drags. Immediately review costs, pricing, and quality. Consider discontinuing loss-making items.
- Boost Office Supplies Margin: Despite high retention, the declining ~3-5% Profit Margin needs attention. Promote high-margin sub-categories (e.g., Paper, Labels) and address inefficiencies in low-margin ones.
- Capitalize on Technology: This category shows strong and increasing 13-14% Profit Margins. Continue investment and innovation.

***-> By aggressively addressing Furniture and Office Supplies profitability and implementing targeted market strategies (leveraging strong markets, developing Africa, and fixing underperformers), the company can significantly enhance its overall profit margin while sustaining strong growth and customer loyalty.***

