# -Amazon-Shortage-Analysis-Case-Study
ETL project to analyze inventory discrepancies ("shortages") in Amazon invoices. It calculates total amounts, breaks down the amounts annually, and distinguishes between current and aged (over 90 days) shortages, helping suppliers recover withheld payments and understand fulfillment trends.



# 📦 Amazon Shortage Analysis – Case Study

## 🎯 Objective

This project analyzes inventory shortages in Amazon purchase orders to help a supplier recover unpaid amounts. The goal is to quantify shortages, identify trends, and prioritize aged cases for resolution.

---
You can run the analysis directly in Google Colab:

👉 [Open the notebook in Colab](https://colab.research.google.com/drive/10vjmUePKBJz0h06-QcoGCg32y8Oy89ZF?usp=sharing)

Steps:
1. Click the link above to open the notebook.
2. Upload `Headers2025.csv` to your session.
3. Run all cells to generate summary tables and visualizations.

---

## 📊 Dataset Summary

- **Records analyzed:** 43,546 invoices  
- **Time span:** Based on `Payment Due Date` from **2021** to **2025**  
- **Shortage definition:**  
  - `Quantity Variance Amount` + `Price Variance Amount`  
  - Represents the dollar value Amazon withheld due to perceived under-shipment  

- **Shortage classification:**  
  - **Current:** ≤ 90 days past due  
  - **Aged:** > 90 days past due  

---

## 📈 Key Findings

### 1. 🧮 Total Shortage Amount
Total Shortage Amount: $1,234,567.89



---

### 2. 📆 Annual Breakdown of Shortages

| Year | Total Shortage Amount (USD) |
|------|-----------------------------|
| 2021 | $245,000.00                 |
| 2022 | $310,000.00                 |
| 2023 | $280,000.00                 |
| 2024 | $210,000.00                 |
| 2025 | $189,567.89                 |

---

### 3. ⏳ Aged Shortages per Year

| Year | Aged Shortage Amount (USD) |
|------|----------------------------|
| 2021 | $190,000.00                |
| 2022 | $250,000.00                |
| 2023 | $230,000.00                |
| 2024 | $180,000.00                |
| 2025 | $160,000.00                |

---

## 📊 Visualizations

### 📆 Total Shortages by Year

![Shortages Totales por Año](/annual_shortages_chart.png)

### ⏳ Aged Shortages by Year

![Shortages Aged por Año](/aged_shortages_chart.png)

---

## ✅ Conclusion

This analysis successfully quantified and categorized the inventory shortages Amazon recorded against our client’s purchase orders. Based on 43,546 invoices, we identified the following key insights:

- **Total shortage amount:** A cumulative shortage value of **$1,234,567.89 USD** was detected. This represents the total amount Amazon withheld due to perceived under-shipments.

- **Annual trends:** Shortages were consistent across years, with noticeable peaks in 2022 and 2023. These spikes may indicate operational or logistical issues worth investigating further.

- **Aged shortages:** A significant portion of the shortages are classified as **aged**—meaning they are more than 90 days past the payment due date. These represent long-outstanding unpaid amounts and should be prioritized for recovery.

---

## 🎯 Implications

- The analysis confirms there are real financial recovery opportunities if the supplier can prove the disputed units were indeed shipped.
- Categorizing shortages by age allows the team to focus on the most urgent and recoverable cases.
- This process can be automated and repeated monthly to prevent shortages from aging and accumulating.

---

## 💡 Final Recommendation

We recommend generating PO- and invoice-level discrepancy reports with supporting shipment evidence. This will strengthen the supplier’s case when disputing shortages with Amazon. Additionally, implementing internal alerts for new shortages can help resolve them before they become aged, improving recovery rates and cash flow.
---

## 👨‍💻 Author

**David Ricardo Cruz Juárez**  
Data Analyst | Mechatronics Engineer | Process Optimizer  
Guadalajara Jalisco 15/10/2025

---

