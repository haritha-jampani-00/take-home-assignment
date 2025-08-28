# 📦 Supply Chain Lead Time Optimization Analysis

## 🔍 Overview

This project analyzes a supply chain dataset containing 250 rows and 10 columns, focused on supplier performance, inventory distribution, and delivery timelines. The primary objective is to identify inefficiencies, evaluate supplier reliability, and estimate cost savings from improving lead times.

---

## 📊 Key Findings

- **Order Distribution:** Orders span from January to April, with March being the busiest month (106 orders) and January the slowest (27 orders).
- **Inventory Imbalance:** 
  - 📍 *New York* had the highest recorded inventory (499 units in April).
  - 📍 *Chicago* had the lowest (1 unit in January).
- **Supplier Performance:**
  - Supplier B had the shortest average lead time (10 days).
  - Suppliers B & C (from San Francisco and Chicago) handled the most orders.
  - Supplier A had the highest rate of late deliveries.
- **Delivery Timeliness:**
  - 50.8% of shipments were delayed.
  - Furniture was the most affected category (58.33% late).
- **Stockouts:**
  - Most frequent in *Dallas*.
  - *Electronics* category was impacted the most, especially during March.

---

## 💸 Cost Simulation

A **10% late delivery penalty** was applied to total cost for each late order. Then, a **10% improvement in lead times per supplier** was simulated.  
This resulted in:

- **Total Late Cost (Before Improvement):** \$836,916.01  
- **Total Late Cost (After Improvement):** \$731,460.53  
- **Estimated Cost Savings:** **\$105,455.48**

---

## ✅ Recommendations

### 🪑 1. Prioritize High-Risk Categories
- **Furniture:** Establish buffer stocks closer to demand centers.
- **Electronics:** Implement a dynamic safety stock policy.

### 🚚 2. Realign Supplier Strategy
- Shift orders away from Supplier A due to poor timeliness.
- Encourage accountability via **penalties and performance incentives**.

### 📦 3. Data-Driven Inventory Planning
- Introduce a **Reorder Point (ROP)** system:
  - Estimate average daily demand.
  - Add a 20% safety stock buffer.
  - Automate triggers for reorder based on projected demand vs. current stock.

---

## 👨‍💼 Managerial Insight

As a supply chain manager, I would:
- Prioritize **forecasting accuracy** during peak demand months (e.g., March).
- Set up **real-time inventory alerts** to prevent stockouts.
- Conduct **supplier performance reviews quarterly**, adjusting allocations as needed.
- Deploy **predictive reorder models** to reduce delays and stockouts by 15–20%.

---

## 📁 Files

- `supply_chain_data.csv` – Raw dataset used
- `supply_chain_analysis.ipynb` – Exploratory data analysis and simulation code
- `Findings_Report.pdf` – Final summarized report
- `README.md` – This documentation

---

## 🛠️ Tech Stack

- **Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
- **Tools:** Jupyter Notebook / Google Colab

---

## 📌 Notes

- Lead times were recalculated using `delivery_date - order_date`.
- Stockouts and late deliveries were analyzed per **warehouse**, **category**, and **supplier**.
- Cost simulation was simplified using a flat 10% penalty model for demonstrative purposes.

---

## 📬 Contact

For questions or collaboration inquiries, please contact:  
**Haritha Jampani** – [LinkedIn](https://www.linkedin.com/in/haritha-jampani/)

