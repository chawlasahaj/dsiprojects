# Understanding online shopper behaviour with machine learning


## Table of contents
1. [About Olist (Business understanding)](#business_understanding)
2. [Data](#data)
3. [Business objectives](#objectives)
4. [Approach](#approach)
5. [Evaluation](#evaluation)
6. [References and links](#references)

## About Olist <a name="business_understanding"></a>
Olist is the largest online department store in Brazil. It connects small businesses from all over country and enables them to sell products directly to the customers using Olist logistics partners. 

## Data <a name="data"></a>
The dataset contains 110k orders from 2016 to 2018 made at multiple marketplaces in Brazil. It allows for viewing an order from multiple dimensions: from order status, price, payment and freight performance to customer location, product attributes and finally reviews written by customers. There is also a geolocation dataset that relates Brazilian zip codes to lat/lng coordinates.

This is real commercial data which has been anonymised and can be found *[here](https://www.kaggle.com/olistbr/brazilian-ecommerce)* in Kaggle.

![Data Structure](https://i.imgur.com/HRhd2Y0.png)
*Data schema*

## Business objectives <a name="objectives"></a>

Through this dataset, I have used various machine learning methods for the following problems -  

1) Segmentation - How can customers be clustered based on their purchase habits? *(Predicted with 93% accuracy) *  
2) Customer Lifetime Value & Churn - How much will a customer bring in future revenue and are they likely to remain with Olist?   *(Within 6% prediction error) *     
3) Customer reviews - Can we predict customer review scores? *(Predicted with 94% accuracy) * 
4) Recommendations - How can we increase user basket size by engaging users more with a recommendation system?  *(Mean average precision - 1.01) *  


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

Order volume peaks in August, sees a sharp decline and picks up just before Black Friday.  


![Product categories](https://i.imgur.com/L8UMhG9.png)

Bed/bath/table is the biggest category by volume.  


![Shopping times](https://i.imgur.com/E4TOK9I.png)

Tuesdays and Thursdays are the most popular days for online shopping, and afternoon (12pm-4pm) is peak shopping time in Brazil.  

![Category-level Shopping times](https://i.imgur.com/nvlbnQj.png)

Sales of automotive category is very popular on Wednesday mornings and computer accessories on Thursday afternoon.  


![Segment differences](https://i.imgur.com/OTyAqPL.png)

Segments derived from RFM analysis using unstructured machine learning. 

![Stark difference in reviews](https://i.imgur.com/VuIsfTT.png)

There is a need to further understand drivers of review scores by segment - to understand the why behind this learning. 

## Please feel free to look at the code for more details on how these figures were derived - as well as the machine learning workflow. 
