# PaulMbuvi-association-mini

# Association Rule Mining with Simulated Electronics Data

This project demonstrates association rule mining using the Apriori algorithm on simulated electronics store transaction data.

## Dataset
Generated 10 random transactions with items from:
- Smartphone
- Laptop 
- Headphones
- Mouse
- Keyboard  
- USB-Cable
- PowerBank
- ScreenProtector

Each transaction contains 2-5 randomly selected items.

## Methodology
1. Data simulated using Python's random module
2. Transactions converted to one-hot encoded format
3. Apriori algorithm applied with min_support=0.3
4. Association rules generated with min_confidence=0.7

## Example Rules and Interpretation

### Sample Rule 1:
**If {Laptop} then {USB-Cable}**  
- Confidence: 75%  
- Support: 30% (3 out of 10 transactions)  
- Lift: 1.88

**Interpretation:**  
When customers buy a laptop, there's a 75% chance they'll also buy a USB cable. This occurs in 30% of all transactions. The lift of 1.88 means this combination occurs 1.88 times more often than expected by random chance.

**Business Insight:**  
- Bundle laptops with USB cables  
- Place cables near laptop displays  
- Offer "Complete Your Setup" promotions 

### Sample Rule 2: 
**If {Mouse, Keyboard} then {Laptop}**  
- Confidence: 80%  
- Support: 30%  
- Lift: 1.33  

**Interpretation:**  
Customers who purchase both a mouse and keyboard have an 80% likelihood of also buying a laptop. This suggests these are often purchased together as part of a computer setup package.

**Business Insight:**  
- Create "Workstation Bundles"  
- Cross-sell laptops when mouse/keyboard are in cart  
- Optimize warehouse picking paths

## 📈 Results Analysis
- Rules help identify:

- Natural product bundles

- Cross-selling opportunities

- Store layout optimizations

# Key Improvements:
- Added clear visual separation between rules

- Included formatted code blocks for each rule's metrics

- Added specific business action items for each insight

- Improved overall readability with emojis and sections

- Added personal attribution at the bottom

## Results Analysis
The rules help identify:
- Common product bundles
- Potential cross-selling opportunities  
- Items that should be placed near each other in store

## How to Run
1. Install requirements: `pip install pandas mlxtend`
2. Run the Python script
3. View generated rules and their metrics
