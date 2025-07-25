# MSCS_634_Lab_6

## Lab Title
**Association Rule Mining Using Apriori and FP-Growth Algorithms**

## Student Information
- **Name:** Murali Krishna Chintha  
- **Course:** Advanced Big Data and Data Mining (MSCS-634-M40) 

---

## Overview

This lab explores association rule mining techniques using the Apriori and FP-Growth algorithms. We apply these algorithms on the **Online Retail dataset** to uncover frequent itemsets and strong association rules, and visualize patterns using Seaborn. A comparative analysis is performed to evaluate the performance and insights derived from both methods.

---

## Dataset

- **Source:** [UCI Machine Learning Repository – Online Retail Dataset](https://archive.ics.uci.edu/ml/datasets/online+retail)
- **Type:** Transactional data from a UK-based online retail store
- **Attributes Used:** InvoiceNo, Description, Quantity

---

## Tools & Libraries

- Python 3.x
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- `mlxtend` (for Apriori, FP-Growth, and association rules)

---

## Steps Performed

### 1. Data Preparation
- Loaded the Online Retail dataset
- Cleaned data: removed nulls, cancellations, and negative quantities
- Transformed transactions into a one-hot encoded basket format
- Visualized most frequent items using Seaborn barplots
- Visualized item co-occurrence with a heatmap

### 2. Frequent Itemset Mining using Apriori
- Applied Apriori algorithm with minimum support = 0.02
- Extracted top 10 frequent itemsets
- Visualized itemsets with support values

### 3. Frequent Itemset Mining using FP-Growth
- Applied FP-Growth algorithm with the same support
- Extracted and visualized top 10 itemsets
- Compared results with Apriori

### 4. Association Rule Generation
- Generated rules using both Apriori and FP-Growth itemsets
- Metrics used: Support, Confidence, Lift
- Visualized rule strength using a confidence vs lift scatter plot
- Interpreted strong and meaningful rules

### 5. Comparative Analysis
- FP-Growth was significantly faster than Apriori due to its tree-based structure
- Both algorithms returned identical frequent itemsets and rules
- Challenges like memory use and data noise were addressed with filtering and top-N limits

---

## Key Visualizations

- **Top frequent items** (`barplot`)
- **Item co-occurrence** (`heatmap`)
- **Frequent itemsets** from both algorithms
- **Association rule strength** (`scatter plot` of confidence vs lift)

---

## Conclusion

FP-Growth proved to be more efficient than Apriori on large transaction data while producing the same rules. Association rule mining is a powerful technique to uncover hidden buying patterns and co-purchased products in real-world retail scenarios.

---
