# Write a Data Science Blog Post

Here is blog post : https://ebulutbaltaci.medium.com/boston-airbnb-prices-predictions-models-7539c238183e


# Installation

For running this project, the most important library is Python version of Anaconda Distribution. It installs all necessary packages for analysis and building models.


# Introducing a Dataset

Data for analyzing trends in Boston's Airbnb is available for free in Kaggle.com and here. This dataset contains data on listings with a huge number of features, user's reviews and calendar info for Airbnb homes in Boston.


# Motivation

This project was created as part of Udacity's Data Scientist nanodegree. Here I have analyzed Boston Airbnb Open Data following CRISP-DM methodology. Airbnb data for other cities have the same format. So the same understandings and code can be applied to Airbnb dataset of any other city.

The business questions which I have tried to answer in this project are as follows:


This project focuses on answering following questions:

What are the most important factors in property valuation?

What are the factors in price determination?

What time of year has the highest rental prices?


# Data Preparation

The target features for analysis are price, review_scores_rating. To proceed with the analysis, data wrangling should be done as this data set is really messy.

1. I had to clean up the values in several columns: the price column had a dollar sign ($) and comma (,) characters and was in object format. 

2. The data types for other columns like the number of bedrooms, bathrooms, accommodates also required a change so they can be used in calculations.

3. City column had a lot of duplicate entries with few case-sensitive entries, space addition issues, etc. All replicates were replaced with a single city code name and this cleaned data was put into a new column called city_cleansed in listings data. City column also had an unusual entry in some native language which was considered for dropping because there was only one entry as such and I was not losing so much data dropping it.


# Language and Frameworks used

Python3, Jupyter Notebook


# Libraries Used

I use Python3. Here are the libraries I used in my Jupyter Notebook:

1.Numpy

2.Pandas

3.Seaborn

4.matplotlib.pyplot

5.matplotlib.dates

6.sklearn.ensemble

7.sklearn.model

8.sklearn.metrics

9.sklearn.linear_model

10.sklearn.model_selection

11.statsmodels.api

12.re

13.folium



# File Descriptions

There is a notebook available here to showcase work related to the above questions and wrangling process. There are 3 data files used to address the above qustions

 - Listings, including full descriptions and average review score
 
 - Reviews, including unique id for each reviewer and detailed comments
 
 - Calendar, including listing id and the price and availability for that day
 

# Result

With our features using a simple linear regression model, we were able to account for about 60% of the variance in Airbnb prices. Thanks to this, we can provide a method for calculating a good starting point for choosing Airbnb price. The more complex methods got a little more precise and aligned with the most important factors, but all agree that the predictions are not perfect and the variance in the data is not taken into account.

While our models do a great job of generalizing prices by features, each listing is unique, and what made the decision to choose airbnb depends on many features that we can’t capture even though Airbnb is doing their best with their models.

What we look at here is a pricing and valuation according to certain data we have. But we do not have factors such as decoration of the house, wall color, etc. When we consider these factors, different results may arise.




# Licensing, Authors, Acknowledgements

Must give credit to Kaggle - Airbnb for the data. Licensing data and other descriptive information at the Kaggle (https://www.kaggle.com/airbnb/boston) available here. Otherwise, feel free to use the code here as you would like!

Thanks to Kaggle and AirBnb for the dataset and Udacity for the course.