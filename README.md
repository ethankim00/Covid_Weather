# Covid_Weather
How does weather affect social distancing and Coronavirus Spread?

## Data
For this project we aggregated a number of data sources that had daily information on different counties in the United States. For each county we used the following data. 
- Weather (scraped from World Weather Online)
  - Sun - the number of hours of sun in a day accounting for cloud cover
  - Rainfall - the number of inches of rain in a day 
  - Temperature - the average daily temperature. 
- Mobility Data (from Google Mobility Insights)
  - Daily Percent Change from baseline is provided for the following categories
    - parks
    - resididential
    - retail
    - transit stations
- Coronavirus Data, source: New York Times
  - Daily case counts
  - Daily deaths due to coronavirus
- Population dentisty in each county 


## Data Processing
The values for weather data were normalized relative to the associated state in order to account for geographic locations with varying weather patterns.
## Modeling
Fitting linear models to predict the mobility indice based of of weather data revealed strong trends. By fitting an LSTM to our data, we were able to model the pattern of exponential growth. 

## LSTM

#Conclusion
Day to day compliance with social distancing measures is highly dependent on weather variables. The number of hours of sun in a day was positively associated with percent change in mobility from baseline while the amount of rainfall was negatively correlated. 
