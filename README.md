# 📊 Payment Acceptance Rate Analysis

---

## 🎯 Objective  
This project investigates the decline in **credit and debit card payment acceptance rates** processed by Globepay for Deel. The goal is to uncover potential causes behind this drop and provide actionable insights to improve payment acceptance.

---

## 🗂️ Data and Methodology  
- Analyzed **acceptance** and **chargeback** reports, focusing on key features such as:  
  - Transaction date  
  - Country  
  - Currency  
  - Transaction amount  
  - CVV provision  
- Conducted **Exploratory Data Analysis (EDA)** including:  
  - Time series analysis  
  - Acceptance rate segmentation  
  - Chargeback trend analysis  
- Focused on the critical period of declining acceptance rates: **February – April**.

---

## 🔍 Key Findings  

### 1️⃣ Overall Acceptance Rate  
> The average daily acceptance rate is approximately **70%**.

### 2️⃣ Time Trend Analysis  

![Acceptance Rate by Day and Mounth](Payment-Acceptance-Rate-Analysis-\Charts\time trend.png)
> A significant dip in acceptance rates occurred between **February and April**, with notable daily fluctuations indicating potential instability or underlying issues.
![Acceptance Rate Heatmap by Day and Month](Payment-Acceptance-Rate-Analysis-\Charts\time trend Heatmap.png)

### 3️⃣ Segmentation Analysis  

The acceptance rate was analyzed across several key segments. The following visualizations illustrate these insights:

- **Weekend vs. Weekday**  
 ![Weekend vs Weekday Acceptance Rate](Payment-Acceptance-Rate-Analysis-\Charts\Weekend vs Weekday.png)
  Acceptance rates remain consistent between weekends (68%) and weekdays (69%), indicating no significant day-of-week effect.  

- **Day of Week** 
 ![Acceptance Rate by Day of Week](Payment-Acceptance-Rate-Analysis-\Charts\by Day of the Week.png) 
  Acceptance rates are stable across all days, ranging from 66% to 74%.  

- **Country**  
  ![Acceptance Rate by Country](Payment-Acceptance-Rate-Analysis-\Charts\by Country.png)
  Acceptance rates vary slightly by country, with minor differences suggesting no major geographical impact:  
  - US: 67%  
  - MX/AE: ~68%  
  - CA/UK: ~70%  
  - FR: 73%  

- **CVV Provided**  
  ![Acceptance Rate by CVV Provided](Payment-Acceptance-Rate-Analysis-\Charts\by CVV Provided.png)
  Transactions without CVV do not significantly affect acceptance rates, potentially due to tokenized or saved card transactions.  

- **Transaction Amount** 
  ![Acceptance Rate vs Transaction Amount](Payment-Acceptance-Rate-Analysis-\Charts\by  transaction amount.png) 
  A slight negative correlation exists between daily acceptance rate and total transaction amount. Higher transaction amounts may trigger stricter payment processor controls.  

### 4️⃣ Chargeback Analysis  
  ![Daily Acceptance Rate and Chargeback Rate](Payment-Acceptance-Rate-Analysis-\Charts\Chargeback.png) 
> A spike in chargebacks preceded the acceptance rate drop, suggesting a trigger.  
> This may indicate Globepay tightened fraud controls, leading to increased declines.  
> *Note:* Limited historical chargeback data restricts definitive conclusions.

### 5️⃣ Rate Calculations  
> Exchange rate calculations appear consistent across all transactions.

---

## 🕵️ Root Cause Hypothesis  

1. **Chargeback-Driven Controls:**  
   - A surge in chargebacks in January likely prompted enhanced fraud prevention, increasing declines from February onward.

2. **High-Value Transaction Screening:**  
   - Days with unusually high total transaction amounts correlate with stricter approval rules and more declines, suggesting manual or system-level flagging.


## 📈 Conclusion  
This analysis highlights potential drivers behind the declining acceptance rate, particularly linking earlier chargeback trends and high-value transaction activity to increased declines.  

