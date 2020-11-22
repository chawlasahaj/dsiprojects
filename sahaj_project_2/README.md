# Predictive Modelling: Housing prices 

For this project I will be playing the part of an independent data analyst who is conducting research on housing prices in order to guide seller listings. 

I will do this by creating a linear regression model based on the Ames Housing Dataset. This model will use a robust dataset in order to predict the selling price of a house (limited to linear regression and regularization only). 

The key business question to answer is -  

<font size = 3 color = "blue"> **In order to guide seller listings in the future, how can we use housing features to predict home sales prices?** </font>

From a data science perspective, we are also interested to know which modeling approaches yield the most accurate predictions of sales price.


# Dataset

This dataset consists of over 2000 entries with 80 features (mixture of nominal, discrete, and ordinal) for properties in Ames, Iowa that were sold between the years 2006-2010. 

In order to understand the dataset better, please do review the detailed description here- http://jse.amstat.org/v19n3/decock/DataDocumentation.txt


# Executive Summary

Brief overview of workflow - 

1) Exploratory Data Analysis: To understand relationships between variables, clean up missing data and standardize dataframes. For numerical features, the linear relationship was examined using a heatmap and correlation coefficients. For categorical data, bar plots were created to visualize the mean Sale Price across categories.   

2) Feature Engineering: To amplify signal of categorical data, such that it reflects more accurately in the regression model. 

3) Data Modelling: For this project, several models were created and iterated upon. Lasso was used to select and narrow down features (as the project requirement was limited to 25-30 variables). Models were evaluated and selected based on RMSE score. Interpretations and recommendations were made based off of the best-performing model (ridge).  

Through extensive data analysis, I have come to a model that is able to account for 91% of the variance in housing prices, and is able to predict housing prices within an error (root mean squared) of $24,000.

### Here are the top 5 features (ranked in order) for sellers to consider when listing houses, in order to achieve the highest selling price -

Combination of overall quality and living area 
Basement Square Footage              
Lot Size                                        
Excellent Kitchen Quality                
Sale Type - New 

Please have a look at the technical notebook (in 'code' folder) for the full process on how this was derived.

## Contents:
 
- Data Import & Cleaning
- Exploratory Data Analysis + Feature Engineering
- Data Visualization
- Data Modelling
- Conclusions and Recommendations