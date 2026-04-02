# ☕ Coffee Shop Sales Analysis — SQL Project

A complete end-to-end SQL project analyzing coffee shop sales data across multiple Indian cities to support data-driven expansion decisions.

---

## 📊 View Full Report
### 👉 [Click here to open the interactive report](https://abhisingh2499.github.io/Coffee-outlet/Coffee_Shop_Analysis_Report.html)

---

## 📌 Project Overview

This project explores transactional sales data from a coffee shop chain operating across major Indian cities. Using MySQL, it answers 10 key business questions to help leadership decide **where to open new outlets**, **which products to stock**, and **how efficiently each city operates**.

---

## 🗂️ Database Schema

The database (`coffee_shop`) consists of 4 related tables:

city ──────────< customers ──────────< sales >────────── products

| Table       | Description                                      |
|-------------|--------------------------------------------------|
| `city`      | City name, population, estimated rent, city rank |
| `customers` | Customer details linked to a city                |
| `products`  | Product name and price                           |
| `sales`     | Transactions: date, product, customer, total, rating |

---

## 📁 Files in This Repository

| File/Folder | Description |
|-------------|-------------|
| `coffee_store.sql` | Complete SQL file — schema creation, data loading, and all 10 analysis queries |
| `data/` | Folder containing all 4 CSV files: `city.csv`, `customers.csv`, `products.csv`, `sales.csv` |
| `Coffee_Shop_Analysis_Report.html` | Project report with business insights and recommendations |
| `README.md` | Project documentation (this file) |

---

## ❓ Business Questions Answered

| # | Question | Key Concept |
|---|----------|-------------|
| 1 | How many people in each city are estimated to consume coffee? | Market sizing (25% of population) |
| 2 | What is the total revenue from the last quarter of 2023? | Time-based aggregation |
| 3 | How many units of each product have been sold? | Product volume analysis |
| 4 | What is the average sales amount per customer in each city? | Customer spend analysis |
| 5 | Cities with population, estimated consumers, and unique customers | Market penetration |
| 6 | Top 3 selling products in each city | Window functions (DENSE_RANK) |
| 7 | Unique customers who purchased coffee in each city | Customer reach |
| 8 | Average sale per customer vs average rent per customer | Cost vs earnings analysis |
| 9 | Monthly sales growth rate per city | LAG() for trend analysis |
| 10 | Top 3 cities for expansion (revenue, rent, customers combined) | Final recommendation |

---

## 🏆 Final Recommendations

Based on the analysis across all 10 queries:

### ✅ Recommended Cities for Expansion

| Rank | City | Reason |
|------|------|--------|
| 🥇 1st | **Pune** | Highest revenue, strong avg spend, moderate rent |
| 🥈 2nd | **Chennai** | 2nd highest revenue, manageable rent, balanced economics |
| 🥉 3rd | **Jaipur** | Highest customer count, lowest rent per customer, very efficient unit economics |

### ❌ Cities Not Recommended

- **Bangalore** — Rent is too high; avg rent per customer is the highest, creating profit margin risk
- **Delhi** — Large market but lower revenue per customer and relatively high rent

---

## 🛠️ Tech Stack

- **Database:** MySQL 8.0
- **Language:** SQL
- **Concepts Used:** JOINs, GROUP BY, CTEs (WITH clause), Window Functions (DENSE_RANK, LAG), Subqueries, Date Filtering, Aggregations

---

## ✅ Conclusion

This project demonstrates how structured SQL analysis can directly inform real business decisions. By examining 10 different dimensions of the data — from market sizing and product performance to unit economics and growth trends — a clear picture emerged of which cities offer the best opportunity for expansion.

**Pune** leads as the top choice with the highest revenue and strong customer spending. **Chennai** follows with solid performance and balanced costs. **Jaipur** rounds out the top three with exceptional unit economics — the highest customer count and the lowest rent per customer make it a highly efficient market.

Cities like Bangalore and Delhi, despite their size and brand appeal, present unfavorable cost-to-revenue ratios at this stage. This analysis shows that bigger markets don't always mean better returns — profitability depends on balancing revenue with operational costs at the city level.
