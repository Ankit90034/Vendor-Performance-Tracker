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
