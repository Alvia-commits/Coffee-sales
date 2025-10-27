1. Introduction

This project aims to analyze coffee sales data using Python to discover useful business insights. Coffee is one of the most consumed beverages worldwide, and understanding customer behavior can help optimize product offerings and increase profits.

The main goals of this project are:

- To identify the most sold coffee type.
- To calculate how much profit each coffee type generates.
- To understand monthly sales patterns.
- To find the peak hours for coffee sales.
- To determine how many customers pay without using a card.

This analysis is useful for café owners, managers, or marketers who want to make data-driven decisions for improving coffee shop operations.

3. Data Cleaning

The data was already mostly clean, but a few minor adjustments were made:
- Combined date and time columns was skipped due to parsing issues — instead, the hour was extracted directly from the time column.
- The monthly_sales column was ignored since it repeated the same value.
- The month and hour values were extracted to help with time-based analysis.
- Card IDs were anonymized, so they were also excluded from the analysis.

📈 4. Exploratory Data Analysis (EDA)

Here are the key questions explored:
a. Which coffee sells the most?
- Answered using value counts on coffee_name.
b. How much profit does each coffee type bring?
- Calculated by summing the money column grouped by coffee_name.
c. Monthly sales trend of each coffee?
- Grouped by month and coffee_name.
d. How many people do not use a card?
- Filtered cash_type != 'card' and counted.
e. What are the peak hours of sales?
- Extracted hour from time, then grouped and visualized.
Visualizations were created using Matplotlib and Seaborn to make the data easier to understand.

✅ 5. Insights and Conclusions

- Best seller: Latte, Cappuccino, Americano with Milk, and Americano.  
- Most profitable: Latte. 
- Peak hour: Most transactions occur around 10 AM to 7 PM, likely due to office work hours.  
- Customer behaviour: Most customers prefer card payment, only 13% use cash.

Monthly trend: [Mention if sales peaked in certain months]

These insights can help the café decide what to promote, when to offer discounts, and how to manage staffing or inventory.
