# Coca-Cola's Stock Analytics Dashboard

For the past three months, I received advice and support from professionals working in technology companies to develop this Coca-Cola Stock Analytics dashboard. This is a personal project I built to put into practice the tools I am currently learning. 

I built this dashboard by pulling the information from [Kaggle Coca-Cola Stock History](https://www.kaggle.com/datasets/kalilurrahman/coca-cola-stock-live-and-updated) public dataset. I used Google Sheets and Dataiku DSS for experiments and parse the dates column. I used Google Looker Studio to create this dashboard to facilitate the decision-making analysis of shareholders (CEO, current employees) and prospectus who are considering investing in Coca-Cola's Stocks. 

Here are a few highlights:

1. Low volatility of the stock price and consistent increase in dividends and high/close prices - this makes it attractive for long-term investments, quantitatively showing a) confidence of the shareholders in the company's management, and b) Coca-Cola's commitment to paying dividends to shareholders.
   
   In comparison with competitors' data, such as PepsiCo, Coca-Cola has performed slightly better in stock splits than 
   [PepsiCo over the last 20 years](https://finance.yahoo.com/quote/PEP/historyperiod1=1035244800&period2=1680134400&interval=1d&filter=history&frequency=1d&includeAdjustedClose=true), which may indicate that Coca-Cola has a stronger growth prospects. 

2. Finding and fixing data quality issues:
   
   a) Extraction - The data was pulled from Kaggle as a .csv file and uploaded on Google Looker Studio to create 
   exploratory visualizations and come up with a series of diagnoses of the challenge and quickly debut. 
   
   b) Transformation - Dataiku DSS supported the analysis of rows and columns, especially on the "Date" column. This is how I
   discovered that there were random clusters of rows in the Date column with different date formats. Further, I noticed that
   weekends and holidays values were missing so I parsed the date column with Dataiku DSS and extracted it as a .csv file. I wrote
   Python code to insert the missing days, added the value of the previous day, and extracted it as a .csv to upload on Looker Studio.

To access the dashboard, click here: [Coca-Cola Stock Analytics dashboard](https://lookerstudio.google.com/embed/reporting/606e64cf-f921-46f8-8f44-fc00c776c883/page/FarED). To access the Python code to solve the missing data challenge, check the attached .ipynb file.

## Coca-Cola Stocks Analytics 

The Kaggle Coca-Cola Stock History dataset ranges from January 2, 1962, to October 26, 2022. The weekends and holidays were missing from the original data. Following domain of expertise principles, I added the missing rows and filled them with the value of the previous row. Some of the information found in this dataset is: 

* Volume Traded
* Dividends 
* High Price
* Close Price
* Stock Splits 

I believe other interesting analyses can be done with this dataset. 

## Questions answered on this dashboard

1. What is Coca-Cola's dividend history?  
2. Does the high price increase or decrease year-over-year (YoY)? 
3. Does the close price increase or decrease year-over-year (YoY)? 
4. How has Coca-Cola performed compared to its industry peers, such as PepsiCo? 
5. Is Coca-Cola's stock history showing reliable long-term investment based on their historical data? 
