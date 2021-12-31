<p align="center">
    <img src="https://github.com/CharlesDeLabra/EDA-Marketing-Campaign/blob/main/allyouneed.jpg?raw=true" alt="Logo" width=72 height=72>
  <h3 align="center">Marketing Campaign Analysis</h3>
  <p align="center">
    This is a EDA Project whose goal was to analize a marketing campaings and give recommendation to the company to improve their campaigns.
    <br>
  </p>
</p>


## Table of contents

- [Context](#context)
- [Problem Statement](#problem-statement)
- [Code](#code)
- [Status](#status)
- [Analysis](#analysis)
- [Conclusions](#conclusions)
- [Recomendations](#recomendations)

## Context

Marketing Analytics broadly refers to the practice of using analytical methods and techniques to understand the effectiveness of various marketing activities and deploy data-driven decisions to optimize for ROI on conversion rates. It typically involves analyzing various metrics around customer engagement with various marketing activities including but not limited to, ATL (above the line) marketing activities, BTL (below the line) campaigns, targeting personalized offers. Typically the variables of interest are customer profile, campaign conversion rates, and costs associated with various marketing channels. These can generate valuable insights that can help an organization form better marketing strategies, optimize/innovate on delivery, and achieve overall growth

## Problem Statement

Company 'All You Need' has hired you as a Data Scientist and you've been told by the Chief Marketing Officer that recent marketing campaigns have not been as effective as they were expected to be and the conversion rate is very low. Your task is to analyze the related data, understand the problem, and identify key insights and recommendations for the CMO to potentially implement.

The data set marketing_data.csv consists of 2,240 customers of All You Need company with data on:

- Campaign successes/failures
- Product preferences
- Channel performances
- Customer profiles based on the spending habits

## Code

The program was written on Jupyter Notebooks in Python Language. You can access to the code [here](https://github.com/CharlesDeLabra/EDA-Marketing-Campaign/blob/main/Learner_Notebook_Project_Marketing_Campaign_Analysis.ipynb)

## Status

The code is finished and have been evaluated, the goal was completed since the conclusions were given to the company in order to them to improve their
campaigns based on the EDA Analysis and the plots and summaries obtained.

## Analysis

First it is needed to understand the dataset, so this summary was presented:
<br>
<p align="center">
    <img src="https://github.com/CharlesDeLabra/EDA-Marketing-Campaign/blob/main/Images/data.JPG?raw=true" alt="Data" width=600 height=650> 
</p>
<br>
Here we can notice that most of the columns are numeric and also that there are no missing values except from income column, since the dataset 
have 2240 entries.

Then we obtained the summary statistics:
<br>
<p align="center">
    <img src="https://github.com/CharlesDeLabra/EDA-Marketing-Campaign/blob/main/Images/statistics.JPG?raw=true" alt="Data" width=620 height=650> 
</p>
<br>
From the statistics we can conclude:

- Most of the clients were born before 1977 with an average born on 1968
- The minimum value on Year_Birth should be wrong because a client can't be born on 1893, so we need to check the outliers of this variable.
- Income have missing values and on average a client has an 52k income but 25% earn less than 35k
- Half or more of the clients last purchase was more than one month ago
- On average clients spend more money on wine (303 USD) than any other product
- Fruit (26.3 USD) followed by Sweets(27 USD) are the products in which clients spend less money.
- On average the purchases made with discount are low (2.6) this is because 75% of clients are from 0 to 3 purchases with discount
- Store purchases still are the most used to buy our products although web purchases are close to store in sales and have a higher maximum with 27 compared to 13 of store.
- Catalog purchases are the least used for our product and most of our clients used them between 0-4 times.
- There is less than one children on average on customer housholds and almost 75% have no one and 25% have at most 2 children
- The same pattern is repeated with teenagers on average there are more than children but on average customers does not have teenager on their household and only 25% of customer have at most 2 and 75% does not have a single.

From the categorical variable we can conclude that:

- 50% of clients are on graduation followed by PhD and Master degrees
- Most of clients are married or have a partner
- Except from second campaign (85%), all of the campaigns have at least 92% of no acceptance
- Most of the clients are from Spain (48%) and less from Mexico (0.13%)

Since the result were to large to present here, it is needed to go to the code part in order to see the implementation of this part.

In order to continue we need to replace some similar categories in some variables, for example in the Marital Status variable it was replaced Alone with
Single, since both of them mean the same.

Then it were created different column in order to have more information that where implicit in the data. The columns that were created were:
- Total spending by a customer
- Total purchase by a customer
- Number of childrens
- Campaign Acceptance


## Conclusions

- The clients who accepted more the campaigns are the one who bought more wine, who doesn't have children and have higher income.
- Clients age is between 1960 and 1980
- Last Campaign was the worst campaign of all
- Second Campaign was the best one
- People with lower income use more deals purchases.
- When the income is higher the clients accept more the campaigns.
- Very high income clients buy with catalog and are less likely to use deals
- Store sales are have the higher number of purchases because it is highly used by everyone
- People with PhD and Master buy a lot of meat and wine.
- Countries spends half of their spending on wine
- People with basic education buy more the othe products.
- Store purchases accepted more campaigns than other channels.

## Recomendations

- Company needs to avoid or improve strategies used in last campaign and use the ones they used on the second one.
- Even that the clients with more income, accepted more the campaigns, it is needed to focus on the medium income based on the distribution of the income which have a median 40k and the values are well distributed around this value.
- It is needed to focus on clients who buy wine and have no children.
- It is a good idea to make a campaign focused on meat and wine products with PhD and Master clients
- It is needed to focus on people with PhD since they are the ones who accept the campain and also buy more wine
- Catalog campaign should be focused on high income clients in order to increase the number of them.
- Campaign 2 had a high value of acceptance with clients with no children, so it will be correct to replicate this.
- Store campaigns can be focused uniformly
- Last campaign didnt affect the acceptance of the one who bought wine so it is needed to focus on the othe products.


