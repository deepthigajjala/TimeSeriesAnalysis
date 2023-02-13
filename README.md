🎈🎈# TimeSeriesAnalysis🎈🎈

❤️❤️##BUSINESS PROBLEM❤️❤️

Ad Ease is an ads and marketing based company helping businesses elicit maximum clicks @ minimum cost. AdEase is an ad infrastructure to help businesses promote themselves easily, effectively, and economically. The interplay of 3 AI modules - Design, Dispense, and Decipher, come together to make it this an end-to-end 3 step process digital advertising solution for all.

You are working in the Data Science team of Ad ease trying to understand the per page view report for different wikipedia pages for 550 days, and forecasting the number of views so that you can predict and optimize the ad placement for your clients. You are provided with the data of 145k wikipedia pages and daily view count for each of them. Your clients belong to different regions and need data on how their ads will perform on pages in different languages.

There’s 1 for dates with campaigns and 0 for remaining dates. It is to be treated as an exogenous variable for models when training and forecasting data for pages in English.

❤️❤️##MY ANALYSIS❤️❤️

1. I imported the data set and did some basic pre-processing on data.
2. I checked this Dataset has 145063 rows and 551 columns.
3. I have seen null values for some websites after some days. I concluded that new websites are created.
4. I dropped the columns which has all null values that means the website not at all visited.
5. I also dropped that websites which has more than 300 null values as they are newly created.
6. After dropping off rows which has some null values there are some null values for existing rows so I filled them using backward fill method.
7. I splitted the Page column as I need to do modelling for only english websites
8. By plotting the graphs I concluded that among all languges English website has more no. of views and Access origin whith all_agents are visited more. Websites with access_type all_acccess are vistied more. Desktop and mobiles websites are vistied equally.
9. Then I grouped the data for each language.
10. Checked for stationarity using ADfuller test.
11. As data is non stationary I removed trend and seasonality by differentaiting.
12. ACF and PACF plots are plotted.
13. I ran ARIMA model and selected best p and q values which has less MAPE.
14. By using obtained best p and q values from ARIMA model I ran SARIMAX model and got best P and Q values.
15. By using the best obtained p,q,P,Q values I ran SARIMAX model and calculated MAPE.
