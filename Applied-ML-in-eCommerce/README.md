# Brazilian e-Commerce Data Analysis

## Table of contents
1. [About Olist (Business understanding)](#business_understanding)
2. [Data](#data)
3. [Business objectives](#objectives)
4. [Approach](#approach)
5. [Evaluation](#evaluation)
6. [References and links](#references)

## About Olist <a name="business_understanding"></a>
Olist is the largest online department store in Brazil. It was founded in 2015 and is based in Curitiba, Brazil. It connects small businesses from all over Brazil to channels and those merchants are able to sell their products through the Olist Store and ship them directly to the customers using Olist logistics partners. After a customer purchases the product from Olist Store a seller gets notified to fulfil the order. Once the customer receives the product, or the estimated delivery date is due, the customer gets a satisfaction survey by email where he can give a note for the purchase experience and write down some comments.

## Data <a name="data"></a>
The dataset has information of 100k orders from 2016 to 2018 made at multiple marketplaces in Brazil. Its features allow viewing an order from multiple dimensions: from order status, price, payment and freight performance to customer location, product attributes and finally reviews written by customers. There is also a geolocation dataset that relates Brazilian zip codes to lat/lng coordinates.

This is real commercial data which has been anonymised and can be found *[here](https://www.kaggle.com/olistbr/brazilian-ecommerce)* in Kaggle.

![Data Structure](https://i.imgur.com/HRhd2Y0.png)
*Data schema*

## Business objectives <a name="objectives"></a>

Through this dataset, I have used various machine learning methods for the following problems -  

1) Segmentation - How can customers be clustered based on their purchase habits?   
2) Customer Lifetime Value - How much will a customer bring in future revenue?  
3) Churn - Which customers are likely to remain or not remain with Olist?  
4) Recommendations - How can we increase user basket size by engaging users more with a recommendation system?  
5) Customer reviews - Can we predict customer review scores based on the various features?


## Approach <a name="approach"></a>

- Data import and wrangling
- Exploratory data analysis
- Time series visualization
- RFM Analysis - with K-means unsupervised machine learning
- RFM Analysis - with lifetimes library and probabalistic BG/NBD Modelling
- Multi-class predictive classification of reviews (positive/negative)
- Product recommendation engine 



## Evaluation and conclusion <a name="evaluation"></a>
A macro level view of the learnings can be found in the Tableau visualization *[here](https://public.tableau.com/views/OlisteCommerceinBrazil/Story1?:language=en&:display_count=y&:origin=viz_share_link)*.


## Key Insights
### Platform-level
![Order volume](https://i.imgur.com/ipwdrX9.png)
*Order volume peaks in August, sees a sharp decline and picks up just before Black Friday.*

![Product categories](https://i.imgur.com/L8UMhG9.png)
*Bed/bath/table is the biggest category by volume.*

![Shopping times](https://i.imgur.com/E4TOK9I.png)
*Tuesdays and Thursdays are the most popular days for online shopping, and afternoon (12pm-4pm) is peak shopping time in Brazil.*

![Category-level Shopping times](https://i.imgur.com/nvlbnQj.png)
*Sales of automotive category is very popular on Wednesday mornings and computer accessories on Thursday afternoon.*

![Segment differences](https://i.imgur.com/OTyAqPL.png)
*After RFM analysis using unstructured machine learning*

![Stark difference in reviews](https://i.imgur.com/VuIsfTT.png)
*There is a need to understand drivers of review scores*
