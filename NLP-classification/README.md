# Project 3: Webscraping, NLP and classification modelling

## Background: 

I am an advertising analyst looking to optimize advertising efficiency. My target audience for this project is people who work in tech support, and my goal is to effectively target this audience using the correct keywords relevant to them.

To this end, I have decided to explore Reddit in order to classify posts, based on natural language processing. For this project, I will be focusing on primarily text-based subreddits to enable more accurate text analysis. To increase the complexity, I will aim to classify posts from similar subreddits to tease out the nuances that make them different.

Thus, the subreddits I have chosen are  
1) https://www.reddit.com/r/talesfromtechsupport/  
2) https://www.reddit.com/r/talesfromcallcenters/

Combined, the 2 subreddits have a total of 800,000 members. Both have a similar purpose, ie - rantings by support departments. Therefore, it will be interesting to see what makes them different, and if machine learning models can accurately classify posts to one or the other. 

For the sake of this project, I will be focusing on accurately classifying posts that belong to the tech support group.

Therefore from a data science perspective the optimization parameter for my model should be accuracy.

## Problem Statement: 


### What are the indicative words that help to effectively target advertising to a niche user group (tech support)? 

## Data Science Challenge: 

### How can I accurately identify posts that belong to 2 subreddits that are very similar in purpose but show differences of nuance?


#### Overview of technical analysis: 

1) Data Scraping and wrangling using Reddit API   
2) Exploratory Data Analysis  
3) Natural Language Processing and Classification Modelling (Logistic Regression and Naive Bayes)  
4) Advanced Modelling with CARTs (Random Forest, Extra Trees, Support Vector Machine, ADA Boost, Gradient Boost) and Optimization 
5) Fresh Reddit scrape for 'true' unseen data  
6) Final Modelling with optimized parameters  

#### In addition to the General Assembly project requirement, I have also looked into a personal area of interest - 

7) Sentiment Analysis and Topic Modelling Visualization (Latent Dirichlet Allocation)   



#### For ease of viewing, I have separated each section into a separate jupyter notebook.

## Executive Summary:

### With an accuracy score of 99.7% on 'true' unseen data, Random Forest classifier is theoretically the best model to answer the data science challenge, as it draws the most accurate decision boundaries for classification. 

### But in my opinion, Logistic Regression is a better model to answer the business problem, as the model is interpretable and I was able to obtain relevant keywords for better targeting. Thus I am confident to proceed with this model to answer the overarching question.