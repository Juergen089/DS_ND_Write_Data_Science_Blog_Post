# Udacity Data Scientist Project #1: Write a Data Science Blog Post

Link to the related blog post on medium:
https://medium.com/@mac_count/examination-of-munich-airbnb-data-4eb5351c1314

# Background

This project is the first project and part of Udacity's Data Scientist nanodegree. The task is to analyze a dataset using the CRISP-DM process. For this purpose I have selected the Airbnb data of my hometown Munich for the period 09/22 to 08/23.

Following business question I tried to answer in this project:
- How does the average rental price for Airbnb offers in Munich develop over the year, using 2022/2023 as an example?
- How does the listing price differ across neighborhoods. What are the most expensive and what are the most affordable locations?
- Can the listing price be predicted based on certain characteristics?

# Used Datasets

The analysis uses the Airbnb dataset from insideairbnb:
- The listings for Munich: http://data.insideairbnb.com/germany/bv/munich/2022-09-21/data/listings.csv.gz. 
- The booking calendar for Munich:
http://data.insideairbnb.com/germany/bv/munich/2022-09-21/data/calendar.csv.gz.
- There is also a description of the columns of the listings file availiable under https://docs.google.com/spreadsheets/d/1iWCNJcSutYqpULSQHlNyGInUvHg2BoUGoNRIGa6Szc4/edit?usp=sharing

All data used in this analysis is also part of this distribution.

# Installation

For this project, Python 3.9 and the Anaconda Package is needed. The Anaconda enviroment file blog_post_env is part of this distribution.

# Content of the Notebook

The distributed jupyter notebook contains the steps data understanding, data preparation & wrangling as well as data modeling.

# Results

It can be noted that the price of Airbnb offers sometimes varies significantly over time. Especially at special events such as large trade fairs or the Oktoberfest, the price rises sharply. The price is also dependent on the location of the offer (district).

With a linear model, such as the scikit-learn ridge regressor used here, and the available data, a satisfactory prediction of the price is not possible. One reason could be the strong temporal variability of the price over time.
It is noticeable that the many coefficients show a high variability over different data sets.
