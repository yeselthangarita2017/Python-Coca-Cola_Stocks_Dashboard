# Python_Missing_data_Coca-Cola Dashboard

From January to March 2023, I received advice and support from professionals working in technology companies to develop this Coca-Cola Stock Analytics dashboard. This is a personal project I built to put in practice the tools I am currently learning. 

I built this dashboard by pulling the information from [Kaggle Coca-Cola Stock History](https://www.kaggle.com/datasets/kalilurrahman/coca-cola-stock-live-and-updated) public dataset. I used Google Sheets and Dataiku DSS for experiments and parse the dates column. I used Looker Studio to create this dashboard to facilitate the decision-making analysis of shareholders (CEO, current employees) and prospectus who are considering investing in Coca-Cola's Stocks. 

Finding and fixing data quality issues:

a) Extraction - The data was pulled from Kaggle as a .csv file and uploaded on Looker Studio to create exploratory visualizations and come up with a series of diagnoses of the challenge and quickly debut. 

b) Transformation - Dataiku DSS supported the analysis of rows and columns, especially on the "date" column. This is how I discovered that there were random clusters of rows in the date column with different date formats. Further, I noticed that weekends and holidays values were missing so I parsed the date column with Dataiku DSS and extracted it as a .csv file. I wrote Python code to insert missing days, added the value of the previous day and extracted it as a .csv to upload on Looker Studio.




To access the dashboard, click here: [Coca-Cola Stock Analytics dashboard](https://lookerstudio.google.com/embed/reporting/606e64cf-f921-46f8-8f44-fc00c776c883/page/FarED). To access the Python code to solve the missing data challenge, check the attached .ipynb file . 

## Coca-Cola Stocks Analytics 

The Kaggle [Coca-Cola Stock History](https://www.kaggle.com/datasets/kalilurrahman/coca-cola-stock-live-and-updated) dataset ranges from January 2, 1962 to October 26, 2022. The weekends and holidays were missing in the original data. Following domain of expertise principles, I added the missing rows and filled them with the value of the previous row. Some of the information found in this dataset is: 

* High price 
* Close price 
* Stock splits 
* Dividends
* Volume 

I believe other interesting analysis can be done with this dataset. 

## Questions answered on this dashboard

1. What are the stock splits per trimester per year? 
2. What are the dividends? 
3. Does the high price increases or decreases year-of-year (YoY)? 
4. Does the close price increases or decreases year-of-year (YoY)? 
5. Is Coca-Cola stock history showing reliable long-term investment based on their history data? 
