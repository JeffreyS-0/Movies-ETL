# Movies-ETL

## Overview
The purpose of this project was to give Amazing Prime a way to pull information from 3 datasets; ratings.csv, movies_metadata.csv, and wikipedia_movies.json, and to keep the dataset that is in PostgreSQL up to date on a daily basis. In order to fulfill Amazing Prime's wish, we had to follow the process of ETL (Extract, Transform, Load). After loading the datasets and extracting the information to our Jupyter Notebook, our next step was to transform the data. How we did this was by cleaning the data from the movies_metadata.csv and wikipedia_movies.json datasets and then merging these two together. After doing this, we side-stepped to our ratings.csv file and quickly cleaned up that one as well. The ratings.csv dataset is so large that it was in our best interest to keep it as a seperate dataset on its own. Once we got done with cleaning the data, all we needed to do from there was load our newly cleaned data into a PostgreSQL database for easy viewing and future data extraction.

## PostgreSQL
As you can see below, we have successfully loaded our data to the PostgreSQL database and we weren't joking when we said the ratings.csv was large. That's 26 MILLION rows of data!

![movies_query](https://user-images.githubusercontent.com/69607218/137644863-ac304fd4-d5f0-45fd-ab1e-069af6f1ea4f.png)
![ratings_query](https://user-images.githubusercontent.com/69607218/137644867-663cdb3b-3e17-4fd6-849c-beeb8bf4285e.png)
