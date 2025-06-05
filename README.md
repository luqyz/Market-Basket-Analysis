# 🛒 Market Basket Analysis with Bread Basket Dataset

This project applies **Association Rule Mining (ARM)** techniques to the `bread basket.csv` dataset to discover interesting patterns and relationships among frequently purchased items in a retail setting. The analysis leverages both **Apriori** and **FP-Growth** algorithms to extract strong association rules that can be used for business insights like product bundling and recommendation systems.

---

## 📌 Objectives

- Load and preprocess transaction data from a retail bakery dataset.
- Transform data into a suitable format for mining (transactional one-hot encoded format).
- Apply the **Apriori algorithm** to discover frequent itemsets and generate association rules.
- Apply the **FP-Growth algorithm** as a faster alternative for mining frequent patterns.
- Visualize support-confidence relationships and rule networks to interpret patterns.

---

## 🛍️ Dataset Overview

- **File**: `bread basket.csv`
- **Source**: (https://www.kaggle.com/datasets/mittalvasu95/the-bread-basket)
- **Description**: Contains real-world transaction data from a bakery. Each row represents an item purchased in a particular transaction on a specific date and time.

---

## ⚙️ Techniques Used

- **One-hot Encoding** with `mlxtend` for transaction data
- **Apriori Algorithm** with minimum support and confidence thresholds
- **FP-Growth Algorithm** for efficient pattern mining
- **Rule Evaluation Metrics**:
  - *Support* – How often items appear together
  - *Confidence* – Probability of seeing the consequent given the antecedent
  - *Lift* – Strength of a rule compared to random chance

---

## 📊 Visualizations

- **Seaborn Scatter Plot**: Support vs. Confidence with lift encoded as hue and size
- **NetworkX Graph**: Interactive association rules graph with nodes and directional edges showing item relationships

---

## 🔍 Insights

- Identify frequently purchased item pairs or sets (e.g., `{Bread, Coffee} → Cake`)
- Discover cross-sell and upsell opportunities
- Understand purchasing behavior over multiple transactions

---

## 🧰 Tools & Libraries

- `pandas` – Data manipulation  
- `mlxtend` – Apriori and FP-Growth implementation  
- `matplotlib`, `seaborn` – Data visualization  
- `networkx` – Graph-based visualization of rules  
- `numpy` – Numerical operations

---

## 📌 Sample Output

- Association rules with high support and confidence
- Visual network of items with strong lift scores
  
  ## 💡 Applications

- Product placement optimization
- Combo deals and targeted promotions
- Recommendation engines for small retailers

---

> 📈 This project demonstrates how classical data mining techniques can provide business value through pattern discovery in transactional datasets.
