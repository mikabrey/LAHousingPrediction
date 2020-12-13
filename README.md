Creating cross relation between foreclosure and unemployment rate.
Current Los angels housing market is difficult to predict.  I hope creating a cross reference between foreclosure and unemployment will some how help predict a house price.   
My targete cliants are early 30th professional who like to goto coffee shop. 

Data acquisition and cleaning
1) City of los angels foreclosure data by zip code form 2015 to 2020
https://data.lacity.org/resource/kde4-k7yx.json
https://data.lacity.org/resource/f37w-ye7d.json
https://data.lacity.org/resource/4sbs-dcfn.json
https://data.lacity.org/resource/r53k-qp8f.json
https://data.lacity.org/resource/e6cg-sqdy.json
https://data.lacity.org/resource/rsxb-x48z.json
2) City of los angles unemployment data by zip 2020 and Total unemployment per month from 1990 to 2020.
   Unenployment LA County 1990 ~
   https://fred.stlouisfed.org/series/CALOSA7URN.xls
   ratehttp://zipatlas.com/us/ca/los-angeles/zip-code-comparison/unemployment-rate.htm
   Used unemploymnet data by zip 2020 to zip code allocation for the Total unemployment per month data. 
   
3) Income and Liability data 2018 by Zip code
https://data.ftb.ca.gov/California-Personal-Income-Tax/Personal-Income-Tax-Statistics-By-Zip-Code/mriu-wsxf

4) Average Condo price by zip. 2015 ~ 2020
http://www.laalmanac.com/economy/ec37c.php
5) Use Folium to find coffee shops venues 
   

Data I used. 
Income and Liability Data -2018 by zip code
#https://data.ftb.ca.gov/California-Personal-Income-Tax/Personal-Income-Tax-Statistics-By-Zip-Code/mriu-wsxf

#Average Home Price by zip LA 
http://www.laalmanac.com/economy/ec37b.php  2015 ~ 2020 by zip code

#downloaded unemployment rate by Zip coode
http://zipatlas.com/us/ca/los-angeles/zip-code-comparison/unemployment-rate.htm

Los Angeles Area Unemployment Rate
https://fred.stlouisfed.org/series/CALOSA7URN
Home Ownership rate
https://fred.stlouisfed.org/series/HOWNRATEACS006037
Home price by avrage seq foot
https://fred.stlouisfed.org/series/AVELISPRI6037
Employee person 
https://fred.stlouisfed.org/series/LAUCN060370000000005

Median Listing Price per Square Feet Year-Over-Year in Los Angeles County, CA (MEDLISPRIPERSQUFEEYY6037)
https://fred.stlouisfed.org/series/MEDLISPRIPERSQUFEEYY6037
Data Cleaning

I have done the exploratory data analysis and done following manipulations on data.

Creating new features
Removing outliers
Transforming skewed features
Checking for multicoliniearity

2) Training machine learning algorithms:

Linear Regression
Ridge Regression
Support Vector Regression
Gradient Boosting Regression
-----

