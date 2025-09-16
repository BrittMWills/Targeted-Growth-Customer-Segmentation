# Targeted Growth: Finding Zomato’s Most Valuable Customer

## 📊 Project Summary
This project analyzes Zomato’s customers to uncover **which segments drive the most value**.  
By looking at **marital status, family size, order frequency, and spending behavior**, we identify patterns that can guide **targeted marketing, loyalty programs, and product design**.  

The analysis combines **data cleaning, calculated fields, segmentation logic, and Tableau dashboards** to tell a complete story.  

---

## 🔗 Project Links

- 📄 [Full Data Analysis Report](https://docs.google.com/document/d/1HgkMbvqVKk1_xZr0QE3YFFQG_thRFLjqEiYYVzIEWsI/edit?tab=t.0)  
- ⚙️ [Decomposition & Methodology](https://docs.google.com/document/d/1xyj6n0t5IWMNqY7XzbiDVx8bfq-EyoFcCJojEZ69tZQ/edit?tab=t.0)  
- 📈 [Tableau Story Dashboard](https://public.tableau.com/app/profile/brittany.williams2558/viz/FinalProjectZomato_17576025703320/Story1)  

---

## ❓ Problem Statement
Zomato needs clearer insights into **how customer segments behave**:  
- Who orders more often?  
- Who spends more per order?  
- Who comes back fastest?  
- How do behaviors shift by weekday vs. weekend?  

Without these insights:  
- Marketing campaigns risk being too broad.  
- Retention programs remain generic.  
- UX features may not align with actual needs.  

---

## 🔍 Research Questions & Hypotheses

### Primary
1. **Spending & Frequency** – Married spend more per order, singles order more often.  
2. **Basket vs. Frequency** – Married = fewer, bigger orders; Singles = more, smaller orders.  
3. **Timing** – Married dominate weekends, singles dominate weekdays.  
4. **Retention** – Singles return more often within 30 days; married return faster if they do.  
5. **Performance Over Time** – Married drive higher AOV; singles with families drive frequency and loyalty.  

### Secondary
- **Family Size Effect** – Bigger households (3+) place more weekend orders.  
- **Offer Effectiveness** – Married prefer bundles, singles respond to free delivery thresholds.  

---

## 🗂 Data Overview
**Users Table** – demographics (User ID, Age, Gender, Marital Status, Family Size, Income, Education, Occupation).  
**Orders Table** – transactions (Order Date, Sales Quantity, Sales Amount, Currency, User ID, Restaurant ID).  

👉 Joined on **User ID** to connect demographics to purchase behavior.  

---

## 🧹 Data Preparation
- Corrected data types (dates, numbers, categories).  
- Converted sales to USD.  
- Extracted year, month, day from order dates.  
- Filled missing values with `Unknown` or `N/A`.  
- Created calculated fields:  
  - Family Size Bucket (1, 2, 3+)  
  - Segment (Marital Status + Family Size)  
  - Average Order Value (AOV)  
  - Orders per Active Month  
  - Revenue per Customer  
  - % Weekend Orders  
  - Days to Second Order  
  - 30-Day Repeat Rate  

---

## 📊 Key Findings
- **Singles with larger families (3+)** are the **most loyal and frequent** segment → high lifetime value.  
- **Married households** spend more per order but order less often.  
- **Weekend ordering is weak overall**, except for Singles with 3+.  
- **Segmentation works**: Married = *High-Spend Planners*, Singles with Families = *High-Frequency Users*.  

---

## ✅ Hypotheses Outcomes
- **Confirmed:**  
  - Married customers spend more per order.  
  - Singles order more frequently.  
  - Singles are more likely to return in 30 days.  
  - Larger families drive more weekend and repeat orders.  

- **Disproved/Partial:**  
  - Married customers do **not** dominate weekend orders.  
  - Speed of repeat was more influenced by family size than marital status.  

---

## 💡 Recommendations
1. **Targeted Campaigns**  
   - Weekend promotions for Singles with families.  
   - Premium bundles for Married customers.  

2. **Retention Programs**  
   - Tiered loyalty system (frequency + spend).  
   - Personalized reminders (push notifications, “1-click reorder”).  

3. **UX Enhancements**  
   - Bulk ordering features.  
   - Highlight weekend bundles in app.  

4. **Offer Testing**  
   - Run A/B tests for free delivery vs. bundle offers across segments.  

---

## 🚀 Next Steps
- **Immediate:** Launch loyalty programs and segment-based marketing.  
- **Medium-Term:** Expand segmentation with cuisine/geography data; track KPIs by group.  
- **Long-Term:** Predictive analytics for churn & personalization; scale internationally.  

---

✍️ **Author:** Brittany Williams – Junior Analyst (Zomato Analytics Team)  
📅 **Date:** September 2025  
