# PaulMbuvi-association-mini

## 🎮 Association Rule Mining – Tech/Gaming Accessories Store

This mini-project simulates a retail store that sells gaming accessories. Using **Association Rule Mining** (Apriori algorithm), we identify which items are often purchased together, enabling better decision-making for marketing, product placement, and recommendations.

---

## 🎯 Objective

To:
- Simulate transactional data from a tech/gaming accessories store (10 transactions)
- Identify frequently purchased item combinations
- Use the Apriori algorithm to discover association rules with:
  - Minimum **support** of 30%
  - Minimum **confidence** of 70%
- Interpret one rule in simple, real-life terms

---

## 🛍️ Dataset: Simulated Gaming Store Purchases

Each transaction represents items bought together by gamers, content creators, or tech enthusiasts.

### **Unique Items Used:**
- Gaming Mouse  
- Mechanical Keyboard  
- RGB Headset  
- USB Hub  
- Webcam HD  
- Mouse Pad XL  
- Gaming Chair  
- Stream Deck  

### **Sample Transactions (10):**
```python
[
    ['Gaming Mouse', 'RGB Headset'],
    ['Mechanical Keyboard', 'USB Hub', 'Gaming Mouse'],
    ['Gaming Mouse', 'RGB Headset', 'Webcam HD', 'USB Hub'],
    ['Gaming Chair', 'Mechanical Keyboard', 'Stream Deck'],
    ['Gaming Mouse', 'Mouse Pad XL', 'Webcam HD'],
    ['Gaming Chair', 'Mouse Pad XL'],
    ['Mechanical Keyboard', 'Gaming Mouse', 'Mouse Pad XL'],
    ['USB Hub', 'Stream Deck'],
    ['RGB Headset', 'Mouse Pad XL', 'Gaming Chair'],
    ['Webcam HD', 'Stream Deck']
]
```

## 🔎 Methodology

- The Apriori algorithm is applied after one-hot encoding the dataset with pandas.

 ✅ Parameters Used:
- Support: 0.3 (30%)

- Confidence: 0.7 (70%)

- Metric: Confidence

Tools used: mlxtend.frequent_patterns.apriori() and association_rules()

## 📊 Sample Rule Generated
Rule:
If a customer buys a Gaming Mouse, they are also likely to buy a Mouse Pad XL.
- Support: 0.3

- Confidence: 0.75

- Lift: 1.50

## 💬 What It Means in Real Life

In 75% of cases where customers purchase a Gaming Mouse, they also buy a Mouse Pad XL.
This suggests that stores could bundle these items, display them together, or recommend them online as “frequently bought together” to increase sales.

## Tools Used
Python 3.12 

pandas

mlxtend

Jupyter Notebook or VS Code




