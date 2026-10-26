Category Type = 'Order Details'[Category] & " - " & 'Order Details'[Sub-Category]
Revenue per Order = 'Order Details'[Amount] *'Order Details'[Quantity]
Sales Category =IF('Order Details'[Amount] > AVERAGE('Order Details'[Amount]), "Above Average",    "Below Average")
Order Count = DISTINCTCOUNT('List of Orders'[Order ID])
Average Profit Delhi = CALCULATE(AVERAGE('Order Details'[Profit]), 'List of Orders'[City] = "Delhi")
Total Sales = SUM('Order Details'[Amount])
YTD Sales = TOTALYTD([Total Sales], 'List of Orders'[Order Date])
Sales target by category , X aixs- Ctegory, y axis- amount;order details
Max Profit Margin by Sub-Category; Legend: Sub-Category from Order Details, Values: Profit Margin from Order Details
Monthly Sales Trend ;Line chart; X-axis order date, y axis amount
Profit vs Quantity by Sub-Category; Scatter chart; X aixs-quantity, y axis profit
Minimum Target by Segment;Multi-row card, Segment, Target
Sales Performance Matrix; Matrix, Category, Month, Actual Sales, Target
Geographic Sales Analysis; Map, City, amount
Sales Distribution by Sub-Category; Treemap, Sub-Category, Amount
Order Count by State; Funnel chart, State, Order Count measure
