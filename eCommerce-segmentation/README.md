# Olist e-commerce Initial Data Analysis

**Lars Tinnefeld**, 2020-11-23

![portrait](https://images.unsplash.com/photo-1522204523234-8729aa6e3d5f?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1050&q=80)

## Table of content
1. [About Olist's (Business understanding)](#business_understanding)
2. [Business objectives](#objectives)
3. [Approach](#approach)
4. [Data](#data)
5. [Data preparation](#preparation)
6. [Data Modelling](#modelling)
7. [Evaluation](#evaluation)
8. [References and links](#references)

## About Olist's <a name="business_understanding"></a>
Olist is for everyone "who wants to sell more and better" and "who wants to attract new customers". As a business in the e-commerce sector, Olist is an online selling platform for small businesses. On Olist's sign-up page a range of shopkeeper profiles is listed which fits the business model. A strong focus is on attracting more customers through a larger market presence. A user satisfaction report helps to address areas of attention. Olist therefore acts as a service provider which is managing the sales process for the shopkeepers. Olist doen't own any of the offered products and is also not managing shipping or inventory.

## Business objectives <a name="objectives"></a>
The goal of the analysis is to extract information that supports Olist's business objectives. These objectives are: Attracting more shopkeepers by enhancing the service and attracting more end-customers through a broader product spectrum and higher satisfaction. The analysis is part of a business case that is looking into expanding Olist's service to also include logistics and warehousing, something Olist is not offering at the moment.
In detail, the analysis is firstly investigating correlations in the order data with the goal to find potentially important insights that can be integrated into the enhanced service. Secondly, the analysis investigates how the business is developing and how dynamic it changes from day to day. This includes also to find extreme events. Thirdly, a prediction about the size of the business for a future scenario needs to be modelled. This all is base of a selection- and definition process for the potential logistic concept, and eventually a business case. Questions that will be answered in this analysis are in detail:
- Are there correlations and patterns in the data which are important for the concept?
- What is the general business trend?
- How dynamic is the operation and are there extreme events which impact logistic process?
- What does the prediction say about the business in two years?

## Approach <a name="approach"></a>
Success criteria for this analysis stage is to answer the above questions with the available data and information. To archive this the following steps and techniques are applied:
- Data import and wrangling
- Exploratory data analysis
- Time series visualization
- Linear regression

Analysis software and libraries:
- Python
- NumPy
- Pandas
- Matplotlib
- Plotly
- Seaborn
- scikit-learn
- datetime

## Data <a name="data"></a>
The provided data set consists of historical order data from 2016 to 2018 and contains 100,000 orders. There are 8 files available. The below data model displays high level the references between these data- and lookup tables. The data was generously provided by Olist under the license CC BY-NC-SA 4.0 and can be found *[here](https://www.kaggle.com/olistbr/brazilian-ecommerce)* in Kaggle.

![Data Structure](https://i.imgur.com/HRhd2Y0.png)
*Data model as provided in Kaggle*

For the current analysis following data files are used:
- olist_orders_dataset.csv
- olist_order_items_dataset.csv
- olist_products_dataset.csv

![ERD1](https://github.com/LarsTinnefeld/olist_ecom_analysis/blob/main/Olist-Analysis_1_ERD.PNG?raw=true)

## Data preparation <a name="preparation"></a>
The notebook "olist_analysis" contains a complete procedure of data checks and cleaning. Applied verification methods:
- Missing data check: 3% missing data were substituted with forward fill, 0.05% of missing SKU dimensions were substitured with mean
- Duplicate records: No duplicates found
- Data formats: Date columns were converted to datetime format

Following data tables were constructed to perform the analysis:
- df_order_items_consolidated (merging of the three original tables)
- df_orders_daily (grouping by date)

![ERD1](https://github.com/LarsTinnefeld/olist_ecom_analysis/blob/main/Olist-Analysis_1_New_tables.PNG?raw=true)

## Modelling <a name="modelling"></a>
For the predictive analysis part linear regression was applied. The date variable was the only input in this analysis. The output (the predicted value) was the total daily order volume (sold units). The predictions were made for a time range from 2017 to 2020. The date format needed to be translated to a numberical format to satisfy the underlying math. The predictions were added as a new column to the data table and visualized in the same time series chart as the original data. R2-scores calculated the accuracy of the model. To increase the prediction accuracy ourliers were removed from the data.

## Evaluation and conclusion <a name="evaluation"></a>
A complete evaluation report is contained in the linked blog post *[here](https://larstinnefeld.medium.com/an-e-commerce-data-story-e53eb8e16f90)*.

### Main conclusion summary
**Are there correlations and patterns in the data which are important for the concept?**
![top_categories](https://github.com/LarsTinnefeld/olist_ecom_analysis/blob/main/Olist_top_categories.PNG?raw=true)

The list contains the top selling categories. The focus can be set on these when optimizing the logistic chain.

![Shipping_metrics](https://github.com/LarsTinnefeld/olist_ecom_analysis/blob/main/Scatterplot%20shipping%20range.png?raw=true)

There is a potential opportunity for including an express ship process in the future logistic concept. The chart shows some relation between shipping duration spread and product price.

**What is the general business trend?**
**How dynamic is the operation and are there extreme events which impact logistic process?**

![trend](https://github.com/LarsTinnefeld/olist_ecom_analysis/blob/main/Time%20series%20overview.png?raw=true)

The business is growing and the day-to-day volume is fluctuating very dynamically. Black Friday is a major event for the business.

**What does the prediction say about the business in two years?**

![prediction](https://github.com/LarsTinnefeld/olist_ecom_analysis/blob/main/Linear%20regression%20design.png?raw=true)

The prognosis is predicting with some error margin that in beginning 2020 in average 500 units per day will be sold.

## References and links <a name="references"></a>

**[Blog post](https://larstinnefeld.medium.com/an-e-commerce-data-story-e53eb8e16f90)**

**[Data in Kaggle](https://www.kaggle.com/olistbr/brazilian-ecommerce)**
