# Vendor-Performance-Tracker

#### Download the data
##### Firstly I have to download the data from the website.
This dataset folder contains six files.
- begin_inventory.csv
- end_inventory.csv
- purchase_prices.csv
- purchases.csv
- sales.csv
- vendor_invoice.csv

#### Understand The Business Problem
##### Effective inventory and sales management are critical for optimizing profitability in the retail and wholesale industry. Companies need to ensure that they are not incurring losses due to inefficient pricing, poor inventory turnover, or vendor dependency. The goal of this analysis is to:

- Identify underperforming brands that require promotional or pricing adjustments.
- Determine top vendors contributing to sales and gross profit.
- Analyze the impact of bulk purchasing on unit costs.
- Assess inventory turnover to reduce holding costs and improve efficiency.
- Investigate the profitability variance between high-performing and low-performing vendors.

##### Combine the .csv files into one centralized database and create a log file script
Now I have to combine these files into asingle file 'inventory_db' using sql script.
Next step is to create a 'logs' folder that contains 'ingestion_db' file.
Using this script further data can be combined.

##### Load the merged file into jupyter
- Now I have to load the merged file into jupyter.
- It is on this file we will be performing data cleaning, data analysis etc.

##### Data cleaning
- Now I will clean the data such as to fix the null values, handle formatting issues such as to convert a column in to proper(e. g. convert the Volume column into 'float64' which is in 'Object' format
- Handle the duplicate values
- Eliminating unnecessary whitespaces from the categorical columns such as VendorName

##### Exploratory Data Analysis(EDA)
- Now I have performed EDA on the cleaned data file.
- During this process I have per
- I also created new features during this phase such as 'GrossProfit', 'ProfitMargin', 'StockTurnover' etc.
- Examined the structure of data using commands such as 'df.describe()'

##### Vendor Performance Analysis
- Here we tried to find the outliers in data.
- Using countplots and correlation heatmap to find the correlation between the columns
- Here we gathered various correlation insights:
  - PurchasePrice has weak correlations with TotalSalesDollars (-0.012) and GrossProfit (-0.016), suggesting that price variations do not significantly impact     sales revenue or profit.
  - Strong correlation between total purchase quantity and total sales quantity (0.999), confirming efficient inventory turnover.
  - Negative correlation between profit margin & total sales price (-0.179) suggests that as sales price increases, margins decrease, possibly due to                competitive pricing pressures.
  - StockTurnover has weak negative correlations with both GrossProfit (-0.038) and ProfitMargin (-0.055), indicating that faster turnover does not necessarily      result in higher profitability.
##### Answer various questions using data such as:
- Identify the brands that needs the promotional or pricing adjustments which exhibit lower sales performance but higher profit margins.
- Which vendors and brands demonstrate highest sales performance?
- Which vendors contribute most to the total purchase dollars?
- How much of total procurement is dependent on top vendors?

##### Recommendations:
- Re-evaluate the pricing for the low sales, high margin brands to boost the sales volume without sacrificing profitability.
- Diversify the vendor partenerships to reduce the dependency on a few suppliers and mitigate the supply chain risks.
- Leverage the bulk purchasing advantages to maintain the competitive pricing while optimizing the inventory management.
- Optimize the slow moving inventory by adjusting the purchase quantities, launching clearence sales, or revising storage strategies.
- Enhance the market and distribution strategies for low performing vendors to drive higher sales volume without compromising the profit margin.
- By implementing these recommendations company can achieve sustainable profitability, mitigate risks and enhance overall operational effieciency.
