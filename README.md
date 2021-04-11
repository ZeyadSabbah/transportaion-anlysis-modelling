# Green Taxi
This project is dealing with dataset provided in this [link](https://www1.nyc.gov/site/tlc/about/tlc-trip-record-data.page) about green taxi trip records include fields capturing pick-up and drop-off dates/ties, and other interesting information.  

The data used is of the month February, 2016 and it took place in NYC.

## Explore
### Data
green_tripdata_2016-02.csv: data is downloaded by running the wrangle_act file
green_taxi_clean.csv: data is written by running the wrangle_act file
nyc_neighbourhoods.json: data collected from data-beta-nyc-files website for neighbourhoods information


## Files
### wrangle_act
Three processes take place in this file.  
1. Gather  
Collecting packages needed for cleaning process and the data.  

2. Assess  
Practicing visual exploration of the data defining the points that might be problems performing the data analysis. This step addresses quality and tidiness issues.  

3. Clean  
Applying different techniques to deal with issues stated in the Assess process in regards of quality and tidiness of the data before moving forward with the data analysis.  

### explanatory_data_analysis
It contains two main parts  
1. Data Preparation  
It is a complementary step to the cleaning process. Further steps were taken to have polished and understandable graphs.   

2. Questions
This part contains answering questions asked to give a clear answers.  
Note: More data about NYC's neighbourhoods was collected.  

### time-series_modeling
It contains of three main parts  
1. Data Preparation
A lot of data preparation was required in order to have it ready for time-series analysis and modeling.  

2. Time-Series Analysis  
Investigating what type of time-series data it is in order to specify which model will work with it the best. It contains seasonal decomposition, ACF, and PACF.  

### Modeling
1. Forecasting  
a) Using grid search techniques using SARIMA for the different hyperparamaters selection.  
Note: The cell containing this step takes long time to run.  
After selecting the best AIC and Log Likelihood, the best model would be one degree higher in terms of AR factor.  

b) Plotting and analyzing results to ensure residuals normal distribution and non-stationarity.  
c) Plotting forecasting vs real points along with confidence interval.

2. Evaluating  
Using RMSE as the main evaluation metric.
