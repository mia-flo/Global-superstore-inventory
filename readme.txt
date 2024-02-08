global super store project (2011-2014)

51,290 initial records and 24 columns


modules used:
-pandas
	-summary statistics of both numerical and categorical features of the data
	-groupby to summarize: metrics by market, number of discounts and at what percent, metrics by product category
		--top markets by sales: APAC, EU, US
		--top markets by profit: same
		--top markets by quantity of units sold: APAC, LATAM, US
		--top categories by profit and sales: technology, office supplies, furniture
	-correlations by region
		--shipping costs were strongly correlated with sales for each region

-seaborn
	-histograms of sales and profit distributions
	-box plots of sales and profit distributions
	-strip plot of shipping method vs sales
		--standard class is the most popular and sees a greater range of sales values
	-linear regrssion plots (lmplot) for sales vs profit generally and sales vs profit by market
	-scatterplot of sales vs profit by discount %
	-linear regression of sales vs profit by discount %
		--<27% discount is correlated with higher profit. higher than that, profit is low to negative
	-linear regression of shipping cost vs sales and profit. profit has a weak to no relationship with shipping cost. sales, 		however, is moderate to strong. 
	-lineplots for time series analysis of the sum of sales amount and the sum of sales numbers by year (2011-2014)
		--peaks in number of sales (6, 9, 11, 12) with sharp drops in July and a drop in September
		--peaks in sales amount (6, 9, 11, 12) with sharp drops in July and a drop in September


-matplotlib
-numpy

-math
	-used to calculate bins and bin widths for seaborn histograms
-scipy
	-used to conduct 1 sample t-tests
		--null hypothesis: discounts are not related to the quantity of units purchased (done on the entire data set and 		by region)
		--the null hypothesis is rejected when looking at the overall dataset. however, when looking at individual 				regions, the null hypothesis is accepted (except for Canada - perhaps they do not offer any discounts?)



regions:

-APAC
-EU
-US
-LATAM
-Africa
-EMEA
-Canada


cleaned and conducted exploratory data analysis that consisted of:
	-data type change
	-checked for duplicates and missing data
	-summary statistics (histograms, bar charts, boxplots) to get a sense of the data distribution
	-correlation analysis using pandas
-linear regression analysis using seaborn and pandas to calculate the r2 value
-time series analysis of order dates using pandas and matplotlib
-t tests

to understand the relationships between discounts, sales, and profit for the different markets that are serviced.