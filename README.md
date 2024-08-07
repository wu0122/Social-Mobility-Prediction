# Social-Mobility-Prediction
Link to github: https://github.com/wu0122/Social-Mobility-Prediction/tree/main

The American Dream is a key tenet of American pride - our country holds itself high as the land of opportunity to drastically improve one’s financial and social standing in a rags to riches story. In this paper, we investigate the degree to which the American Dream holds true and how its conditions have evolved since 1984, focusing on the degree to which social mobility is available to low-income households. In order to provide insight into how America could improve its vertical mobility, poverty rate, and overall prosperity, we use several models to analyze the effect of several key measures across other high income countries and provide predictions for how key changes in those measures would affect the country. The variables used to characterize social mobility include median income, house price, disposable income, the GINI index, tuition costs, education quality and access, welfare spending as a % of GDP, monthly Medicare premiums, percent of children that earn more than their parents, and the share of wealth by the top 1% compared to the bottom 50%. This study provides linear models, LASSO models, relaxed LASSO models, trees, and random forest models for predicting social mobility, poverty rate, and GDP per capita, but chooses to use backwards-selected linear models for predictions for America for greater explanation of variables, confidence intervals, and lowest error for Social Mobility and Poverty Rate, but a Relaxed LASSO model for GDP Per Capita for minimizing error. This study provides a crucial look into the current condition of financial upwards growth for the current and future generations as well as recommendations for where the country should focus on learning from other high income countries for restoring the promise of the American Dream. This research opens the door for following research to look into how such policies and recommendations could be implemented and their real effects. 

This program imports data from the data folder within the zip folder, subsets for non-NA value rows only, and graphs variables against Social Mobility Index, Poverty Rate, and GDP Per Capita for correlation. Additionally, it analyzes data on the US for Gini Coefficient, Monthly Medicare Premiums, House Price, Share of Wealth by Top 1% and Bottom 50%, and Percent of Children earning more than their Fathers in three time series graphs. Afterwards, the program sets aside 5 country observations from the original 24 for testing and creates LM, LASSO, Relaxed Lasso, Tree, Random Forest, and XGBoost models for the three response variables. Then, the program calculates Mean Squared Error for each model based on testing data, plots them as bar graphs, and then moves on to analyze with the least MSE models for the three response variables. After creating dataframes based on the most correlated variables changed to predict the changes for three seperate hypothetical USA's. These hypothetical USA's are based on the variables being decreased/increased according to this:

The values were chosen based off of other countries’ real values in these variables, and created 3 different changed Americas to predict off of: 1, 2, and 3 representing a midball improvement, a best case scenario, and a worst case scenario respectively. It should be noted each model does not use all 8 variables. To create midball, we took the average of original and highest value in each variable then rounded to nearest country, then took same amount and decreased for the lowball.

The predicted values of Social Mobility Index, Poverty Rate, and GDP Per Capita are displayed with 95% confidence intervals for the three hypothetical US's in seperate dataframes.

The following are references, although all necessary data is already within the zip.

Board of Governors of the Federal Reserve System (US). (1989a, July 1). Share of Total Net Worth Held by the Bottom 50% (1st to 50th Wealth Percentiles). FRED, Federal Reserve Bank of St. Louis. https://fred.stlouisfed.org/series/WFRBSB50215

Board of Governors of the Federal Reserve System (US). (1989b, July 1). Share of Total Net Worth Held by the Top 1% (99th to 100th Wealth Percentiles). FRED, Federal Reserve Bank of St. Louis. https://fred.stlouisfed.org/series/WFRBST01134

Data. (2018, July 24). Opportunity Insights. https://opportunityinsights.org/data/?geographic_level=0&topic=0&paper_id=546#resource-listing

Digest of Education Statistics,. (n.d.). Nces.ed.gov. https://nces.ed.gov/programs/digest/d23/tables/dt23_330.10.asp

FRED. (2016). GINI Index for the United States. Stlouisfed.org. https://fred.stlouisfed.org/series/SIPOVGINIUSA

FRED. (2018). Real Median Personal Income in the United States. Stlouisfed.org. https://fred.stlouisfed.org/series/MEPAINUSA672N

FRED. (2023). Consumer Price Index for All Urban Consumers: All Items. Stlouisfed.org. https://fred.stlouisfed.org/series/CPIAUCSL

Here’s Why Medicare Part B Premiums Have Increased Over Time. (n.d.). The Balance. Retrieved August 1, 2024, from https://www.thebalancemoney.com/current-and-historical-medicare-part-b-premiums-2388483

U.S. Bureau of Economic Analysis. (1947, January 1). Personal saving as a percentage of disposable personal income. FRED, Federal Reserve Bank of St. Louis. https://fred.stlouisfed.org/series/A072RC1Q156SBEA

U.S. Federal Housing Finance Agency. (1975, January 1). All-Transactions House Price Index for the United States. FRED, Federal Reserve Bank of St. Louis. https://fred.stlouisfed.org/series/USSTHPI

Degenhard, J. (2021, July 20). Gini index worldwide 2020, by country. Statista. https://www.statista.com/forecasts/1171540/gini-index-by-country

Income share of the richest 1% (before tax). (n.d.). Our World in Data. Retrieved August 1, 2024, from https://ourworldindata.org/grapher/income-share-top-1-before-tax-wid?tab=table&time=1820..latest

Numbeo. (2023). Health Care Index by Country 2019 Mid-Year. Numbeo.com. https://www.numbeo.com/health-care/rankings_by_country.jsp

Poverty rate. (n.d.). OECD. Retrieved August 1, 2024, from https://www.oecd.org/en/data/indicators/poverty-rate.html?oecdcontrol-0ad85c6bab-var1=CHE%7CSWE

Social Mobility by Country 2021. (n.d.). Worldpopulationreview.com. https://worldpopulationreview.com/country-rankings/social-mobility-by-country

The Education Price Index 2022 — a Study by N26. (n.d.). N26.com. https://n26.com/en-eu/the-education-price-index

Transparency International. (2024). 2023 Corruption Perceptions Index. Transparency.org; Transparency International. https://www.transparency.org/en/cpi/2023

Wikipedia Contributors. (2019, September 6). List of countries by social welfare spending. Wikipedia; Wikimedia Foundation. https://en.wikipedia.org/wiki/List_of_countries_by_social_welfare_spending

World Population Review. (2021). Education Index by Country 2023. Worldpopulationreview.com. https://worldpopulationreview.com/country-rankings/education-index-by-country

Worldometer. (2023). GDP by Country. WorldoMeters. https://www.worldometers.info/gdp/gdp-by-country/


