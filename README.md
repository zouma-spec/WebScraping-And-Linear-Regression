WebScraping & Linear Regression
Topic: Deep dive into computer monitor pricing
Computer monitor is a major productivity tool for people whose work requires long time sitting in front of the computer. As a data practitioner or prospective data practitioner, you probably have or are searching for a right monitor for you. Best Buy as one of the top electronics retailer, offers multitudinous monitors to customers. While as customers, we might feel overwhelmed when facing with so many features and so many options of monitors. One might wonders what feature(s) of monitors is(are) the main driving factor(s) of determining the prices of monitors? Thus, my analysis is focusing on exploring what features of monitors affect the prices and, predicting the price of a monitor given its features.

Abstract
This project is to use regression to predict computer prices in order to help people make wiser purchasing decisions. I scraped monitor data from Bestbuy.com including monitor prices as target and monitor specifications/features as features and fit regression model on the data. I built linear regression model on the data and step by step refined he model. I increased r score value from 0.616 of a baseline linear regression model to 0.816 of an Elastic Net regression model.

Design
The focus of my project is to fit a optimal linear regression model with best r score I can get and to find the biggest predictor.

Data
I scraped data of monitor from the Bestbuy.com twice(once a week), and originally got 1102 data points. The point of scraping data twice from different time is monitor prices/rating might change over time. After data cleaning and wrangling, duplicate data got dropped and I ended up with 502 data points, indicating monitor picing/rating didn't change.



Algorithms
Baseline OLS model on numeric features using statsmodels to have intuitive understanding of the data
Implement Feature Engineering
Linear Regression using scikit-learn and implement cross validation to avoid overfitting
Continue fit linear regression on categorical variables using One Hot Encoding
Regularization (landed on Lasso regression as the best model)
Tools
Web scraping: BeautifulSoup selenium requests
Data cleaning/analysis/modeling: pandas numpy sklearn statsmodels scipy.stats
Data Visualization: matplotlib seaborn
Communication
5 minute slide presentation
