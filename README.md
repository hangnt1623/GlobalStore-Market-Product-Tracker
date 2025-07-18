# 📊 Market Expansion & Product Strategy for Sales using PowerBI

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
This project analyzes **global sales performance** of **Superstore** using provided datasets (**Orders**, **People**, **Returns**). The objective is to:

- Provide an overview of the company's **business situation**: This includes understanding overall **sales trends**, **revenue**, and **profitability**  
- Support **market expansion strategies**: By identifying **top-performing regions**, **untapped markets**, and **customer segments**  
- Inform **strategic product selection**: By analyzing **product performance**, identifying **best-sellers**, and understanding **customer preferences**


### 👤 Who is this project for?  

✔️ Senior Manager of Superstore (mainly)

✔️ Sales and Marketing Teams  

✔️ Product Development Teams 

✔️ Regional Managers

✔️ Business Analysts

###  ❓Business Questions:  

✔️ Understand overall **business performance** by analyzing **sales**, **profit**, and **quantity trends** over time and across different segments  

✔️ Identify **high-potential markets** for expansion and areas requiring **strategic intervention** based on **regional performance**  

✔️ Pinpoint **strategic products** by evaluating **profitability**, **sales contribution**, and **return rates** of various **product categories** and **sub-categories**  

✔️ Provide **actionable insights** and **recommendations** through an interactive **Power BI dashboard** to support the **Senior Manager's decision-making process**


### 🎯Project Outcome:  
**1. Market Expansion**
- **Prioritize Investment:** APAC (**high revenue, good margin, high retention**), EU (**highest profit, reduce returns**), and Africa (**near 0% returns, high potential**)
- **Review & Reassess:** Canada (**high margin but 93% churn**), LATAM (**low profit/revenue, high risk**), and US (**large scale, but retention/returns suboptimal**).


**2. Strategic Products**
- **Technology (Accessories & Phones):** Expand portfolio, boost marketing, control costs.  
- **Office Supplies:** Maintain stability, no large-scale expansion needed; focus on high-profit groups.  
- **Furniture:** Restructure (cut/adjust weak groups); stop expansion if no improvement.

**3. Customer Segments (Bonus)**
- **Corporate:** Prioritize retention (**high profit, stable purchases**)  
- **Consumer:** Improve shopping experience (**high return rate**)  
- **Home Office:** Explore upsell strategies (**good retention, low revenue**)


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

**1️⃣ Empathize**

***(1) 5W1H***

<img width="685" alt="{CE7A0D03-D63F-4DE9-A25C-8C33F0AAE397}" src="https://github.com/user-attachments/assets/a3b3a7e5-27c4-4ec9-92b2-ea419f2006c3" />

<img width="685" alt="{8D425E12-81E5-4E4F-9BF5-F7C290C555C3}" src="https://github.com/user-attachments/assets/7e8fa7c0-0b93-4e6d-9d15-dd622f8d0a35" />


***(2) Empathy Map***

<img width="687" alt="{D87110DB-1A5F-40D3-B7A6-BB9755758910}" src="https://github.com/user-attachments/assets/1a621ac3-3aac-4e54-b913-bc031c8575b1" />

***(3) Stakeholder need***

<img width="685" alt="{54A28E57-1A7C-4D18-B8A0-3C02CC9DAE0B}" src="https://github.com/user-attachments/assets/cf9b985e-f85f-41dd-b7e1-7f792b331d9e" />


**2️⃣ Define point of view**  

***(1) North Star Metric***

<img width="689" alt="{2C521022-6453-4AB3-976F-194D09C3E5D4}" src="https://github.com/user-attachments/assets/a9194e90-059f-4439-af1b-61b93a1d36f5" />

***(2) Point of view***

<img width="686" alt="{145BC1D8-98CA-41D3-89F2-5D6356703D75}" src="https://github.com/user-attachments/assets/5f0cdb09-34a7-4a54-99a2-6e385244eb8f" />


**3️⃣ Ideate**

<img width="689" alt="{43661513-A425-4A30-8D55-B371D77A030B}" src="https://github.com/user-attachments/assets/f9971def-fc52-4088-a067-803a5e76e7ee" />

---

## 📊 Key Insights & Visualizations  

### 🔍 Dashboard Preview & Analysis

#### 1️⃣ Dashboard 1: Overview

<img width="755" height="418" alt="{E8180417-602E-492B-AFB4-560240C78584}" src="https://github.com/user-attachments/assets/c2c28d8e-50ba-4dce-ad03-e707dbf44b16" />

📌***Oberservations***
- **Overall Financial Health:**
  + Superstore shows robust performance with 51.55% YoY Revenue Growth and a solid 11.61% Profit Margin. Low Return Rate (4.69%) and high Retention Rate (92.23%) further reinforce operational effectiveness and customer satisfaction.

- **Sales Are Seasonal, But Profitability Isn't Always Synced**
  + Sales exhibit consistent seasonal patterns (Q4 peak, Q1 dip)
  + yet Profit Margin fluctuates significantly quarterly, not consistently reflecting sales volume. For instance, Q4 profit margins varied widely across years despite consistent sales peaks.
  + -> While sales seasonality is clear, profit optimization during peak and off-peak periods is inconsistent, requiring better alignment of strategies and costs.

- **Furniture: A High-Sales Category with a Profitability Problem**
  + Technology leads in profit and sales. However, Furniture, despite being the second-largest sales contributor, yields disproportionately low profit due to its starkly low 7% Profit Margin (vs. ~14% for other categories).
  -> Furniture's low profitability acts as a significant drag on overall profit, demanding an urgent review of its cost structure and pricing.

- **Market Strategy: Focus on Proven Winners, Address Underperformers**
  + APAC, EU, and US are top-performing markets with strong sales and healthy margins. Conversely, EMEA struggles with a low 5.45% Profit Margin. Canada, though boasting a 26.62% Profit Margin, has negligible sales, indicating a high-risk, unscalable niche
  + -> Prioritize expansion in proven strong markets while critically addressing profitability issues in EMEA. Approach Canada with caution due to high risk relative to its current scale.

- **Home Office Segment: Profitable Yet Prone to Churn**
  + The Home Office segment is highly valuable with the highest 11.99% Profit Margin and lowest 4.40% Return Rate. However, it also surprisingly has the highest 8.21% Churn Rate.
  + -> Despite high initial value and satisfaction, Superstore struggles to retain Home Office customers. Targeted retention strategies are crucial to maximize their long-term value.

  
📌***Recommendations***
- **Optimize Seasonal Profitability**: Implement dynamic pricing and cost controls to ensure consistent profit margins across all seasons, especially during Q4 peaks.
- **Boost Furniture Profit**: Conduct an urgent cost and pricing review for Furniture to significantly improve its low 7% profit margin.
- **Prioritize Core Markets; Fix EMEA**: Maximize growth in APAC, EU, and US. Urgently restructure EMEA operations to address its low 5.45% profit margin.
- **Retain Home Office Segment**: Develop targeted programs to reduce the 8.21% churn rate in the highly profitable Home Office customer segment.


#### 2️⃣ Dashboard 2: Market Analysis

<img width="757" height="420" alt="{A7F20A9A-3AD5-4CBD-A435-27AECFDB7B4A}" src="https://github.com/user-attachments/assets/ee3f3b2b-5079-4c20-8fb4-95984203ea8e" />

📌***Oberservations***
- **Market Profitability: Persistent Disparities Across Regions Over Time**
  + Profit Margins show distinct, consistent patterns across markets over four years (2011-2014).
  + Canada consistently holds the highest Profit Margin (ranging 21.24% - 25.88%), while EMEA consistently records the lowest (ranging 3.87% - 7.49%).
  + APAC and EU maintain stable profit margins with low volatility, reflecting their maturity, while Africa and LATAM show steady annual growth in their margins.
  + -> The long-term trends confirm inherent, structural profitability differences across markets. Canada's high margin, despite very low sales volume, persists. Conversely, EMEA's consistently low margin signals deep-seated challenges that are not improving over time.
- **Core Markets Drive Volume, While Extremes Highlight Opportunities and Risks**
  + APAC, EU, and US are Superstore's volume leaders, dominating in Total Orders (e.g., APAC has 5.4K orders, 27x Canada's 201 orders) and generating substantial sales.
  + Consumer customer segment consistently accounts for the highest sales across all seven markets, confirming its overall importance.
  + On the other end, Canada consistently has the lowest sales volume across all customer segments, yet maintains its top-tier profit margin.
  + -> Volume is concentrated in established markets, led by the Consumer segment. The extreme contrast of Canada (tiny volume, high margin) versus other markets confirms it as a unique, potentially risky niche rather than a scalable growth engine.
- **Varying Efficiency and Loyalty Across Markets: The Return & Churn Story**
  + While APAC boasts the highest total orders, its Return Rate (5.46%) is notable.
  + EU, despite being the fourth largest in orders, records the highest Return Rate (6.21%).
  + In stark contrast, EMEA, Africa, and Canada, which have the lowest order volumes, also show exceptionally low Return Rates (0.04% - 0.50%).
  + However, this low return rate in Canada is overshadowed by an alarming 93.44% Churn Rate, which is by far the highest. Africa (46.59%) and EMEA (40.85%) also exhibit significantly high churn.
  + -> High return rates in key markets like EU indicate potential product fit or expectation management issues that can erode profitability. More critically, Canada's extremely high churn, despite its high profit margin and low returns, points to a severe customer retention problem – customers might buy, be satisfied initially, but rarely repurchase. Similarly, the high churn in Africa and EMEA signals fundamental issues in sustaining customer loyalty, impacting long-term viability in these markets.


📌***Recommendations***
- **Sustain & Optimize Strong Markets**
  + APAC: Continue investment to leverage scale and 12.16% PM
  + EU: Prioritize reducing its 6.21% Return Rate to maximize the 12.69% PM
  + US: Focus on improving retention and reducing its 5.95% Return Rate to solidify 12.47% PM.
- **Develop Africa's Retention**: Invest in strategies to boost retention and reduce churn in Africa, capitalizing on its good 11.34% PM and minimal returns
- **Strategic Review for Challenging Markets**:
  + LATAM: Optimize operations and address its 5.82% Return Rate to enhance its 10.24% PM
  + EMEA: Requires a major strategic overhaul to address the 5.45% PM and very high churn
  + Canada: Investigate the extreme churn (93.44%) despite high 26.62% PM; unsustainable for growth


#### 3️⃣ Dashboard 3: Product Analysis

<img width="757" height="417" alt="{F79ADC7B-AEF3-46A7-879A-694D2F79C180}" src="https://github.com/user-attachments/assets/e3c163f0-b870-4ba3-81af-b4879942c838" />

📌***Oberservations***
- **Core Category Performance**:
  + Office Supplies dominates order volume (>50%)
  + Furniture consistently shows the lowest, volatile Profit Margin, contrasting with more stable Technology/Office Supplies.
  + -> Furniture's low profitability is a core issue requiring attention.
- **Subcategory Deep Dive**:
  + "Stars": Copies, Appliances, Bookcases (high growth/profit).
  + "Drains": Tables (negative profit), Envelopes, Papers, Furnishings, Machines (low growth/profit).
  + Tables also have the lowest PM (-8.46%); Paper boasts the highest PM (24.24%).
  + -> Optimize the portfolio by pushing "Stars" and re-evaluating "Drains" based on their specific performance.
- **Operational & Segment PM Consistency**:
  + Return Rates are stable annually (approx. 4.5%-4.8%).
  + Home Office has the highest Profit Margin (11.99%), but only marginally better than other segments.
  + -> Stable returns confirm operational consistency. Product strategy should prioritize category performance over minor segment PM differences.


📌***Recommendations***
- **Amplify "Star" Subcategories & Leverage Office Supplies Dominance**:
  + Increase investment (marketing, inventory, potential R&D) in high-growth, high-profit subcategories like Copies, Appliances, and Bookcases.
  + Strategically cross-promote these with Office Supplies, given its >50% order volume dominance, to drive higher-margin sales.

- **Prioritize Furniture Profitability Turnaround**:
  + Launch an urgent deep-dive into Furniture's cost structure (sourcing, logistics, returns) and pricing strategies.
  + Systematically identify and address specific sub-categories like Tables (-8.46% PM) that actively erode profits, considering either price adjustments, design overhaul, or discontinuation.

- **Strategically Manage Low-Performing Subcategories**:
  + Conduct a rigorous cost-benefit analysis for "Drain" subcategories (e.g., Tables, Envelopes, Papers, Furnishings, Machines - those with low growth/profit/negative profit). <Decisions could include discontinuation, price adjustments, or sourcing optimization.>
  + For Machines specifically (low PM but potentially high absolute profit), focus on margin improvement without sacrificing volume.

- **Develop Product Bundles for High-Value, High-Churn Segments**:
  + Create attractive product bundles or loyalty programs specifically for the Home Office segment, combining high-margin "Star" subcategories (e.g., Copiers, Bookcases) with essential Office Supplies.
---

## 🔎 Final Conclusion & Recommendations  

> **The company demonstrates strong growth and customer loyalty, yet the overall 11.61% Profit Margin is significantly weighed down by underperforming product categories and specific markets.**

👉🏻 Based on the insights and findings above, we would recommend Senior Manager to consider the following:  

**📌 Market Recommendations**
- **Sustain Strong Markets:** Keep investing in APAC, EU, and US. For EU and US, focus on **reducing return rates to maximize profit**  
- **Develop Africa's Potential:** With **good profit and low returns**, prioritize **improving retention and reducing churn** to unlock growth  
- **Overhaul Challenging Markets:**  
  + **EMEA:** Major strategic overhaul needed due to **very low Profit Margin (5.45%) and high churn**  
  + **Canada:** Investigate **extreme churn (93.44%) despite high profit**; it's unsustainable → Approach Canada cautiously with niche testing, not broad expansion.  
  + **LATAM:** Optimize operations and address **return rates**


**📌 Product Recommendations**
- **Launch an urgent profitability turnaround** for Furniture, especially Tables.  
- **Invest in and cross-promote "Star" subcategories** (Copies, Appliances, Bookcases).  
- **Develop targeted bundles for Home Office** to boost retention (8.21% churn).


**📌 Customer Segment Recommendations**
- **Prioritize Home Office Retention:** Implement targeted loyalty and engagement programs for the Home Office segment to address their high **8.21% churn rate**, despite their leading **11.99% Profit Margin**.  
- **Optimize Consumer Segment for Volume:** Refine marketing and offerings for the Consumer segment to maintain its **highest sales across all markets**.  
- **Maintain Product-Centric Profitability:** Focus on optimizing overall product category profitability, as **profit margins across customer segments are very similar**.

