In this project, we will analyze the whole price inflation of India against the wholesale prices of certain crops cultivated between the period of Jan 2013 to Dec 2024.Ofcourse whole sale price inflation and whole sale crop prices are related given that infaltion is calculated using crop prices. But crop prices are not the only factor determining the inflation. Inflation calculation also includes oil & gas price, interest rates, demand/suppply, macro/micro economic factors etc. What we will see in this project is the proportion of variance in inflation exaplained by the variance in the crop prices i.e. how much variance in inflation is caused by fluctuation in crop prices.

Whole sale crop prices are taken from Kaggle Datasets:
https://www.kaggle.com/datasets/samithsachidanandan/wholesale-price-index-from-2012-to-2024

Inflation data is taken from :
https://in.investing.com/economic-calendar/indian-wpi-inflation-564

There are prices of various crops; since some crops could be seasonal, we take mean/sum of crop prices for comparison.
When we plot scatter plot between inflation and price, there is some form of linear relationship with outliers.

The attached jupyter notebook has the data processing and model fit details.
from the results summary, we find that the r squared value for this regression between inflation/price is around 0.415 i.e, more than 40% of variance in inflation is explained by the prices data. This is significant considering only crop prices because we did not include other major factors like oil & gas etc.

In future we could include monsoon rainfall, temparature and humidity data to perform the regression. We beleive that results will provide an idea about the usage of water for cultivation of crops and subsequent inflation
