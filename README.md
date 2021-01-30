# project_2
Team Name: Mean Guacamole Team Members: Melissa Smashey, Kevin Ricker, Krystal Dodd

Project_Data Trump Twitter Insults: https://www.kaggle.com/ayushggarg/all-trumps-twitter-insults-20152021Avocado Prices: https://www.kaggle.com/neuromusic/avocado-prices
Extract: Krystal (Time Estimate 25 minutes)

1). Import dependencies and set up config files. 2). Pull csv files into pandas and rename. 3).  Preliminary investigation 4). Transfer notes for data changes to be made. Notes: Data was take from Kaggle and then imported into a jupyter notebook. The data was examined using print and describe functions to review the data set so I could communicate with Melissa transformations to be made. 

  Issues:  No issues with the data but did have issues pushing to the repository this was because I was not added as a user. 
  
  Transform:  Melissa (Time Estimate 30 minutes to 1 hour) – Went longer than expected this took about 1.5 hours of our time for data cleaning1). Drop unnecessary columns. 2). Reformat data if needed. 3). Merge new dataframes together. Ensure matched.Notes: It was noted in the Extract portion what data points were necessary for our dataframe. WE decided the values we wanted to keep were “Date” “Average Price” and “Total Value”.There was also an index column in the data set this was dropped.
  
    Issues:  We noticed the avocado data had multiple locations included in the data set, this created an issue for any relational data. We decided to group bythe date and then take the average of the average price and sum the total sum so we would have one value by location. We also ran into issues while 
trying to join in pandas. We did not note that one of the dates we were joining on was a text.  We converted this to panadas date format and then was able to join. We dropped the NA values and now ready to load. 

Load: Kevin (1 hour)1). Using the config create engine to postgres 2). Create database in Postgres3). Create Tables in post gres 4). Insert transformed data frames into postgres 5). If more time create our own API call using mongo 

  Issues: We ran into issues when connecting to our database with the conifg password and username files. This was a syntax error that we had difficulty realizing. We then had issues when creating and sending the data to postgres. We had to change columns names as this was affecting our import. When the data was loaded we had issues writing our query this was another syntax error. 
