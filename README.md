# MarketDataScience

In my role as an Investment Analyst at DA Davidson I was responsible for creating a market wide investment analysis tool with over 750 metrics, one and a half million data points, 1500 regression models, and an equation to quantify risk and return metrics. To do this, I used Bloomberg, Excel, R, and Tableau to compare different metrics against one another to assess their risk and return profiles in various risk and return categories such as volatility, leverage, geopolitics, growth, sentiment, valuation, yield, and macroeconomic conditions. An example of this model would have been to quantify if Chinese debt levels are risky relative to historic terms, but then to also be able to compare their debt levels to US debt levels based on how the data was quantified. Because of this, the model created an overview of both equity and bond markets in such a manner that any two metrics are immediately comparable and are given quantified values based on their short term and long term Relative Strength Index, the average of their standard deviations over a five year and ten year period, their coefficient of determination against a relevant benchmark, a test of statistical significance, and then discounted by their reporting period to make more frequently published data more relevant in the model. Through this, we could aggregate up from specific categories such as Domestic Equity Risk Volatility, to a broader category such as Domestic Equity Risk, and still be able to compare it to other categories such as High Yield Fixed Income Risk. Once the calculations had been done in Excel, Tableau was useful as a data manipulation and visualization tool, to create a clear framework for which metrics and categories showed greater risks or returns than others based on the sizing and coloring of the boxes within the treemaps that the data was displayed in. This also allowed for the static model to be turned into a tool with multiple levels that could be navigated through based upon the preferences of the user. The user could navigate through four separate levels, the first being an overall aggregate of the significance and normality of both the bond and equity markets within high yield fixed income, investment grade fixed income, domestic equities, and international equities. The second level was then a breakdown of the subcomponents of the bond and equity markets into the risk and return categories that were assigned to high yield fixed income, investment grade fixed income, domestic equities, and international equities. The third level then took a risk or return category and dived into the specific categories that made it up. For example, domestic equity return would consist of growth, sentiment, valuation, yield, and macroeconomic conditions. From there, choosing a category such as domestic equity return growth, would lead to a screen revealing the individual metrics that made up the category, a graph showing the change in the metric over time, and their RSI, standard deviations, coefficient of determinations, and their reporting period. 
While making this model I utilized data mining, data modeling, and statistical analysis to screen and quantify relevant metrics. Through testing which metrics were relevant with correlations to the overall market, I identified which metrics should be emphasized within the model. Here, issues emerged with heteroskedasticity, where an inconsistent error term emerged due to different observations having different error variance, and multicollinearity, where data was too closely correlated to each other in multiple regressions leading to high amounts of noise and a danger of overfitting the model. Overall, the best regression models are those in which the predictor variables each correlate highly with the dependent variable, but correlate at most only minimally with each other. Therefore, I used individual regressions instead of multiple regressions due to the issues multiple regressions caused with multicollinearity, which lead to unreasonably high coefficients of determination and statistical significance on virtually every metric tested. 
