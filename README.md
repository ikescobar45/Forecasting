I continued my research using the Daily Climate Time Series Data of the City of Dehli.

https://www.kaggle.com/datasets/sumanthvrao/daily-climate-time-series-dataLinks to an external site.

This time instead of focusing on temperature. I focused on humidity.

The data was usable. However, I did have to change the date column to date time.

1.  I plotted the Daily Humidity to see if I could identify any trends. I noticed that the lowest humidity was in the middle of the year, and humidity starts to decrease in January.

Screenshot 2024-09-28 114530.jpg

2.  Then, I used the ADF test to test for stationarity. I achieved a  'p-value' of 0.004470100478130746. Because the p value is less than .05, we can assume the data is stationary, and proceed with an ARMA model.

3.  Next, I plotted the ACF and the PACF of the humidity series. You can see both the graphs spike at 1. Hence, we can use the value of 1 for both P and Q.

Screenshot 2024-09-28 120010.jpg

4. I created the model using 1 for the value of p and q. Below are the model details:

Screenshot 2024-09-28 120641.jpg

5. Lastly, I created the forecast for the next thirty days once the data ends. You can see that the forecast follows the trend of decreasing starting in January.

Screenshot 2024-09-28 120837.jpg
