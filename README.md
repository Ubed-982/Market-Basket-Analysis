# 🛒 Market Basket Analysis using Apriori and FP-Growth

This project explores Market Basket Analysis on retail transactional data from the United Kingdom, Germany, and France. It applies **Apriori** and **FP-Growth** algorithms to extract frequent itemsets and generate association rules, using Python and Spark MLlib.

---

## 📂 Files

| File | Description |
|------|-------------|
| `Market Basket Analysis.ipynb` | Jupyter Notebook with full implementation |
| `Market Basket Analysis.html` | Rendered version of the notebook (view via nbviewer link below) |

🔗 **View Notebook Online (if GitHub can't render HTML):**  
👉 [View HTML notebook on nbviewer](https://nbviewer.org/github/Ubed-982/Market-Basket-Analysis/blob/main/Market%20Basket%20Analysis.html)

---

## ❓ Problem Statement

Efficiently extract meaningful association rules from large transactional datasets.  
**Goal:** Identify the most frequent itemsets and strong association rules by country (UK, Germany, France) and compare the performance of Apriori vs FP-Growth.

---

## 🔍 Research Question

> What are the most frequent itemsets and strongest association rules per country, and how do the Apriori and FP-Growth algorithms compare in terms of performance and scalability?

---

## 📊 Key Results

- **Apriori (min support 5%)**
  - 1,200 frequent itemsets
  - Execution time: ~35 seconds

- **FP-Growth (same threshold)**
  - 1,250 frequent itemsets
  - Execution time: ~15 seconds

- On validation and test sets:
  - FP-Growth retained speed and discovered deeper item associations
  - Apriori slowed down with larger datasets

---

## 🔄 Comparative Analysis

### Apriori Algorithm

- ✅ **Strengths**: Simple, interpretable, works well on smaller datasets  
- ❌ **Limitations**: Slower with larger data due to iterative candidate generation

### FP-Growth Algorithm

- ✅ **Strengths**: Faster execution, better memory usage, scalable with FP-Tree  
- ❌ **Limitations**: More complex to implement and understand

---

## 🧠 Practical Considerations

1. **Data Quality**: Clean and complete data ensures accurate patterns  
2. **Parameter Tuning**: minSupport and minConfidence need careful adjustment  
3. **Scalability**: FP-Growth outperforms for large datasets  
4. **Privacy**: Ensure anonymization and data protection compliance  

---

## ✅ Recommendations

### 1. 🎯 Targeted Marketing
- **UK**: Leverage detailed patterns for personalized promotions
- **Germany/France**: Use top item combos to tailor campaigns

### 2. 🛒 Product Placement
- Place commonly co-purchased items together (e.g., wine + cheese)

### 3. 📦 Inventory Management
- Use real-time trends to avoid stockouts or overstocking

### 4. 💼 Promotions & Bundling
- Create discounted bundles from frequent itemsets

### 5. ⚙️ Algorithm Choice
- **UK (large data)**: Use FP-Growth  
- **Germany/France**: Apriori is sufficient for now

---

## 🔮 Future Work

- Integrate real-time Market Basket Analysis in POS systems  
- Apply analysis to customer segments  
- Extend to other domains like healthcare, finance  
- Explore hybrid models (Apriori + clustering)

---

## 🧾 Conclusion

Market Basket Analysis using Apriori and FP-Growth reveals actionable insights into customer purchasing behavior.  
- **Apriori**: Better for smaller or simple datasets  
- **FP-Growth**: Scales better and uncovers deeper patterns

Retailers can harness these techniques to optimize layout, inventory, and promotions — ultimately improving sales and customer satisfaction.

---

## 📫 Contact

For questions or collaboration:
**Ubed Ullah**   
[GitHub Profile](https://github.com/Ubed-982) | [LinkedIn](https://www.linkedin.com/in/ubedullah)

---

