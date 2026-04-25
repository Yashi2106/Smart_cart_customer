# SmartCart Customer Segmentation
I looked at customer data from SmartCart to figure out who their shoppers really are. The goal? Help them send the right offers to the right people.

## The Data
2,240 customers. Info about what they buy, how much they earn, their family situation, and how they shop.

## first step
Cleaned things up first:
- Filled in missing income numbers
- Created an age column 
- Combined education levels into simpler groups (Undergraduate, Graduate, Postgraduate)

**Finding patterns 
- Rich people spend more. Income and total spending had a 0.79 correlation.

#Grouped similar customers together:
Used K-Means clustering. After testing different numbers, 4 groups made the most sense.

## group wise Customers?

Group 0: High income, spend a lot
Group 1: Middle income, average spenders  
Group 2 Lower income, spend less, have kids at home
Group 3: Older, been customers for a while, like catalog shopping

##Conclusion for buisness

- If someone has money, they'll probably spend it with you
- Families with kids are tighter with their budget
- Long-time customers have different habits than new ones
- Single vs. partnered people shop differently

```bash
pip install pandas numpy seaborn matplotlib scikit-learn kneed
jupyter notebook Smart_cart\(cluestring\).ipynb
