Introduction and Problem Statement

  The goal of the analysis is to help us understanding the relation between unemployment rate/ income/ foreclosure and how zip code are used to determine it.  I hope that creating a model will help predict foreclosure in near future.  I also create recommended zip code for the home seeker in his early thirties who likes to go to coffee shops and like outdoor sports.

Data acquisition and cleaning (Data 

City of los angels foreclosure data by zip code form 2015 to 2020 
  urlf2020='https://data.lacity.org/resource/kde4-k7yx.json?$limit=100000&$offset=0'
  urlf2015='https://data.lacity.org/resource/f37w-ye7d.json?$limit=100000&$offset=0'
  urlf2016='https://data.lacity.org/resource/4sbs-dcfn.json?$limit=100000&$offset=0'
  urlf2017='https://data.lacity.org/resource/r53k-qp8f.json?$limit=100000&$offset=0'
  urlf2018='https://data.lacity.org/resource/e6cg-sqdy.json?$limit=100000&$offset=0'
  urlf2019='https://data.lacity.org/resource/rsxb-x48z.json?$limit=100000&$offset=0'
Total unemployment per month from 1990 to 2020. 
  https://fred.stlouisfed.org/series/CALOSA7URN.xls
Unemployment LA County 1990 
  https://fred.stlouisfed.org/series/CASTHPI
Income and Liability data 2018 by Zip code 
  url='https://data.ftb.ca.gov/resource/mriu-wsxf.json?$where=county="Los Angeles" and taxable_year = 2018 limit 1000000'
Average Condo price by zip. 2015 ~ 2020
  wikiurl ="http://www.laalmanac.com/economy/ec37c.php" 
Use Foreclosure to find coffee shops and sports venues

Methodology section

Updating missing data using data and fill data by using averagae allocation methord. Creating new data frame for data analysis.

Training machine learning algorithms
Initially, I used Multiple Linear Regression,  because, I want to use multiple variable.  I did not get good result, therefore
I tried Gradient boosting regression, it can benefit from regularization methods that penalize various parts of the algorithm and generally improve the performance of the algorithm by reducing overfitting. Also used Ridge Regression to reduces the standard errors. 

Result Section:
Multiple Lineare regresstion has low R-score and high MSE, Redge regression has better result. GradientBoostingRegressor create best result.
R-score close to 1.0. 
Discussion:
  I did not apply seasonal cost adjustmet and infreation adjustment. Next,step will be applying those factor in.
Also, I will use SQL to create initial dataframe. Finding, error using python is just take long time. because, I am very new to python.
Conclusion:
  Out of three model GradientBoostingRegressor create best result.
Most of bank foreclosed house on beginning of year. Maybe because of holiday back log.
When unemployment rate is real high (example 15% or more), foreclosure will not impact unemployment_rate. 
Unemployment between 6 to 10 % impacted foreclosure.
Probably, most of unemployed person do not own the house. Also, I found few good zip code for Venues.

