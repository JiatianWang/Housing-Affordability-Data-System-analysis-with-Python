# Housing-Affordability-Data-System-analysis-with-Python

My purpose is to use a linear regression model to predict the future market value of the properties.

The data is from “Housing Affordability Data System” of the US department of Housing and Urban development [HADS]. I have datasets from 2005 to 2013. Each dataset has the same housing level variables include a number of rooms in the housing unit, locations, the years it was built, Occupied or vacant, rented or owned, single-family or multi-family structure, number of units in the building, market value, monthly housing cost, number of people living, household income, type of residential area, market value, which are up to 26 variables. Each dataset has over 40,000 observations.

I merged all the separated datasets, dropping the unimportant variables, and explored various descriptive statistics summary. I also made visualizations of market values changes overtime in lineplot, how are the market values distributed in boxplot, the correlations between numeric variables in heatmap, scatterplot.
I used natural logarithm to transform my dependent and independent variables for increasing linearity in my model. I found out that the market value in the past, the monthly housing costs, monthly rental fee, location of the housing unit would significantly impact the market value in the future.

Variables correlations in Heatmap:

![heatmap](https://user-images.githubusercontent.com/32876600/108638447-4e566f00-745d-11eb-8867-987d284258b5.png)

Non-transformation, Semi-log regression, Log-log regression:

![3](https://user-images.githubusercontent.com/32876600/108638555-db012d00-745d-11eb-9ae5-0778a8aa15e3.JPG)

After applying logarithm transformation on dependent and independent variables due to lack of linearity in the model, I compared non-transformation (41%), semi-log regression (34%) and log-log regression (60%) on R-square, the more optimizing model can predict 60% accuracy on house market price.

Prediction:

![Regression](https://user-images.githubusercontent.com/32876600/108638608-08e67180-745e-11eb-9ebf-11a0dfb4b270.png)
