# -Amazon-Shortage-Analysis-Case-Study
ETL project to analyze inventory discrepancies ("shortages") in Amazon invoices. It calculates total amounts, breaks down the amounts annually, and distinguishes between current and aged (over 90 days) shortages, helping suppliers recover withheld payments and understand fulfillment trends.



# 📦 Amazon Shortage Analysis – Case Study

## 🎯 Objective

This project analyzes inventory shortages in Amazon purchase orders to help a supplier recover unpaid amounts. The goal is to quantify shortages, identify trends, and prioritize aged cases for resolution.

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

## 💡 Recommendations

- **Prioritize aged shortages**: Focus recovery efforts on invoices older than 90 days.
- **Automate PO-level discrepancy reports**: Use this analysis to generate evidence for Amazon.
- **Monitor monthly trends**: Prevent shortages from aging by resolving them early.

---

## 📁 Repository Structure




---

## 👨‍💻 Author

**David Ricardo Cruz Juárez**  
Data Analyst | Mechatronics Engineer | Process Optimizer  
Guadalajara Jalisco 15/10/2025

---

