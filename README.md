# Movies_ETL

## Overview
Use the Extract, Transform, Load (ETL) process to create data pipelines. A data pipeline moves data from a source to a destination, and the ETL process creates data pipelines that also transform the data along the way. Analysis is impossible without access to good data, so creating data pipelines is often the first step before any analysis can be performed. Therefore, understanding ETL is an essential skill for data analysis. Within the scope of the Amazing Prime Hackathon, this project will create an automated pipeline that takes in new data, from Wikipedia data, Kaggle metadata and the MovieLens rating data. 
For this analysis, we used the following breakdown:

- Write an ETL function to read three data files,
- Extract and transform the Wikipedia data,
- Extract and transform the Kaggle and rating data,
- Load the data to a PostgreSQL Movie Database.

## Results
Write an ETL function to read three data files
The function takes the Wikipedia JSON, the Kaggle metadata and MovieLens csv files and creates three separate DataFrames.

Extract and Transform the Wikipedia data
We filtered out the TV shows, consolidated the redundant data, removed the duplicates and formatted the Wikipedia data.

Extract and Transform the Kaggle and rating data
Again, we consolidated the redundant data, removed the duplicates, formatted, and grouped the data.
The Kaggle and rating data were then merged with the Wikipedia movies DataFrame.


Create the Movie Database

![2022-06-26 (6)](https://user-images.githubusercontent.com/103701561/175834723-7ab1f866-5366-43b3-af81-dfb22f8b702e.png)

## Summary
The ETL function created collects and cleans movie data from three different sources, Wikipedia JSON, Kaggle, and ratings csv files. It transforms and merges the data and loads it into two updatable PostgreSQL dataset tables ready to be used by the hackathon participants for their analysis.
