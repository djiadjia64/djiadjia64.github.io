---
layout: post
title:      "Linear Regression Project"
date:       2020-03-09 07:06:51 +0000
permalink:  linear_regression_project
---


I created a linear regression model for this project. The dataset in question maps the houses in King County in Washington state. Along with the prices of the houses were a multitude of variables, predictive or not. My goal generally was to find the predictive variables and apply them in a model to return a formula that can predict housing price. There was a lot of noise generally in the dataset. After looking through a scatter matrix and plotting out relationships, I only came up with five significant variables at the end. 

It was a lot more challenging of a project than I had initially thought. As I had already done work with combining and editing dataframes in pandas, I was pretty confident that the data cleaning or data manipulation in general was not going to be too bad. I, however, came into problems when it came to trying to interpret the data. The dataset itself was not too bad. There were incomplete values for some of the variables but nothing that did not impede me for significant amounts of time. It took me awhile to come up with the significant variables. Though the process was simple, I was stuck for some time for some reason. Also, changing the data to make the model work properly was challenging in that I had little experience with it generally. I went through a bunch of the normalization and standardizing techniques and took awhile to decide on one. The concept on standardizing vs normalization was also harder for me to grasp, which lenghtened my time in interpreting my data and applying my functions. Once I got the variables sorted out and normalized, I ran into troubles with my OLS regression function. My coefficients were off because I did not normalize price, and my R-squared value was surprisngly low. My conditional number was very high unsurprisingly. Though my R-squared was low, I decided to procede and adjust my variables for multicollinearity. It was not hard to narrow down my correlated variables to those with square feet measurements. I simply normalized all the data and combined the datasets and averaged them to account for the number of datasets combined. Doing this greatly reduced my conditional number in subsequent testing. Afterwards, I validated the model by running cross validation on it. The mean errors returned were all similar and in an acceptable range and verifying my model. Ultimately, I ended up with an R-squared value of 0.487. Not the best but certainly not the worst. Maybe I should have taken out grades as that column did not seem to offer predictive qualities on par with the other variables. 

The other questions I had for the dataset were a little bit easier to tackle. To find out whether the year of renovation of relevant, I simply charted out the year vs. price as well as running the data through a regression test. The results returned were unspectacular. The R-squared value was extremely small at 0.01, and the scatter plot showed no definite correlation. The next question was whether there was a pattern on a heatmap of the county sorted by price. The visual returned from the chart was very interesting and informative. You could easily tell where the affluent areas were and also where the poorer suburbs lie. 

Though I was able to build a model that predicted price to some degree, the model is limited strictly to houses in the King County area. Also, my R-squared was not the best, and my model could definitely use some improving on. 

It was good to be able to reuse some of my skills I had learned in the previous project. It definitely brought some confidence knowing that these skills were very transferable and relevant generally. I had troubles understanding some of the statistical parts of this section as I had never taken a statistics class before. However, I feel a lot more confident about both my skills and understanding in statistics, having done such a hands-on application of it. 




