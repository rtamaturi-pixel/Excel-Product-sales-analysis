#Excel - Product Sales Analysis Project

##Project Overview
This project demonstrates comprehensive Excel data analysis skills applied to a sales dataset. The analysis covers data cleaning, trend identification, customer segmentation, purchase channel performance, and key business metrics.
Key Results: Analyzed 443 transactions (₹213,550 total sales), identified top channels/customers, calculated AOV ₹482

1. Data Cleaning
•	Converted raw data to Excel Table (Ctrl + T) for dynamic referencing.
•	Applied Rupee currency formatting to Purchase Amount (Ctrl + Shift + 4).
•	Added Status column: "Yes" for transactions with purchase amount, "No" for blank.

2. Trend Analysis
•	Created Pivot Table (Insert > Pivot Table).
•	Date in Rows, Purchase Amount in Values for daily sales trends.
•	Removed Quarter/Year groupings for date-level detail.
•	Added line chart for visual trend representation.

3. Specific Customer Analysis - Subbarao
•	**=COUNTIFS(Sales[First Name], C2)** → 7 transactions.
•	**=SUMIFS(Sales[Purchase Amount], Sales[First Name], C2)** → Total spend.
•	**=MAXIFS(Sales[Purchase Amount], Sales[First Name], C2)** → Highest purchase.
•	**=MINIFS(Sales[Purchase Amount], Sales[First Name], C2)** → Lowest purchase.
•	**=FILTER(Sales, Sales[First Name] = C2)** → Full transaction data.

4. Purchase Mode Analysis
•	Pivot Table: Purchase Mode in Rows, Amount and Txn ID in Values.
•	Finding: Website highest (₹81,070, 182 txns); Phone In lowest (₹14,575, 26 txns).
•	**=COUNTIFS(sales[Purchase mode], G4:G7, sales[Status], "Yes")** → Successful transactions.
•	**=J4# / I4#** → Success % with conditional formatting.

5. Customer Analysis by Profession
•	Pivot Table: Job Title in Rows, Amount in Values, Month/Year in Columns.
•	Purchase Mode slicer for filtering.
•	Finding: Professors highest (₹35,225); Administrators lowest (₹1,610).

6. Final Analysis
•	Average Order Value: Total Sales / Successful Transactions.
•	Top 5 products based on revenue and status based on successful transactions have been identified.
•	Top 5 Customers based on the revenue and the status based on successful transactions have been identified.
•	Success rate by each Profession of customers have been identified, this analysis helps us with the targeted marketing.


Tools Used:
Data Cleaning	Excel Table
Analysis	Pivot Tables, Slicers
Formulas	COUNTIFS/SUMIFS/MAXIFS/FILTER
Visualization	Line charts, Conditional formatting


