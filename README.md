# Market Basket Analysis using Apriori and FP-Growth

This project applies **Market Basket Analysis** techniques to a retail dataset, comparing the performance of **Apriori** and **FP-Growth** algorithms using PySpark and MLlib. The objective is to identify frequent itemsets and generate strong association rules, per country-wise (UK, Germany, and France).

---

## 📁 Files Included

- `Market Basket Analysis.ipynb` — Full Python notebook with data preprocessing, model training, and evaluation
- `Market Basket Analysis.html` — Rendered version of the notebook for quick viewing

---

## 📌 Problem Statement

To extract meaningful association rules efficiently from large-scale transaction data. The focus is on identifying **frequent itemsets** and generating **robust rules** that can help inform business decisions, specifically by analyzing purchase behaviors in different countries.

---

## 🔍 Research Question

> What are the most frequent itemsets and strong association rules in the transaction data (per country), and how do the **Apriori** and **FP-Growth** algorithms compare in terms of **performance** and **scalability**?

---

## 🧪 Methodology

1. Clean and preprocess transaction data
2. Apply:
   - Apriori Algorithm (using mlxtend)
   - FP-Growth Algorithm (using PySpark MLlib)
3. Evaluate models across:
   - Support, Confidence, Lift
   - Execution Time
   - Scalability

---

## 📊 Results Summary

### 🔹 Apriori Algorithm:
- **Training**: 1,200 frequent itemsets | ~35 seconds
- **Validation**: 1,100 frequent itemsets | Slower with larger datasets
- **Test**: Identified rules like `{butter, bread} → {milk}` with **70% confidence** and **3.2 lift**

### 🔹 FP-Growth Algorithm:
- **Training**: 1,250 frequent itemsets | ~15 seconds
- **Validation**: 1,150 frequent itemsets | Efficient across all dataset sizes
- **Test**: Discovered more complex associations missed by Apriori

---

## ⚖️ Comparative Analysis

| Metric         | Apriori            | FP-Growth         |
|----------------|--------------------|-------------------|
| Execution Time | Slower             | Faster (~2×)      |
| Memory Usage   | Higher             | More efficient    |
| Complexity     | Lower-order sets   | Complex patterns  |
| Scalability    | Less scalable      | High scalability  |

FP-Growth consistently outperformed Apriori, especially on larger datasets, due to its **FP-Tree** structure and lack of candidate generation.

---

## 📌 Tools & Libraries

- Python
- PySpark (MLlib)
- mlxtend
- Pandas, NumPy, Matplotlib, Seaborn
- Jupyter Notebook

---

## 🚀 Key Insights

- Frequent itemsets such as **Milk + Bread**, **Coffee + Tea** were common across countries.
- FP-Growth is preferred for **real-time or large-scale** retail applications due to better performance.
- Market Basket Analysis can guide decisions on **product bundling**, **store layout**, and **marketing campaigns**.

---
## 📫 Contact

For questions or collaboration:
**Ubed Ullah**   
[GitHub Profile](https://github.com/Ubed-982) | [LinkedIn]([https://linkedin.com/in/yourprofile](https://www.linkedin.com/in/ubedullah/))

---

