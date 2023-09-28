# Movie-Correlation-with-Python

## Aim and Background

The aim of this project was to find movie correlations between variables using Python. I looked at correlations in the data to find the fields highly correlated with the gross revenue. The aim was to find the things that impact the revenue of a film. As part of the analysis I looked at the genre, gross revenue of the movies and release date. This was part of a project by Alex the Analyst.

## About Dataset

There are 6820 movies in the dataset (220 movies per year, 1986-2016). Each movie has the following attributes:

budget: the budget of a movie. Some movies don't have this, so it appears as 0

company: the production company

country: country of origin

director: the director

genre: main genre of the movie.

gross: revenue of the movie

name: name of the movie

rating: rating of the movie (R, PG, etc.)

released: release date (YYYY-MM-DD)

runtime: duration of the movie

score: IMDb user rating

votes: number of user votes

star: main actor/actress

writer: writer of the movie

year: year of release

## Data Cleaning

* I started by exploring the data and reviewing the first 5 rows of the dataframe using the head() function.
* I then reviewed the dataframe to see if there was any missing data. From the output, I could see that a few of the columns had null values (rating, budget, gross, company and runtime).
* After reviewing the column with null values, I then reviewed the data types for each column using dtypes. There are some object data types, intergers and floats. I noted that for some columns there was an additional .0 at the end. In order to get rid of this, I changed the data type for the budget and gross columns to an integer.
* A new "year" column was then created based on the year the movie was released. This was because the year in the released column and in the year column did not match. In order to correct this, a new year column was created to correctly reflect the year each movie was released.
* The data was then ordered by gross revenue in descending order. Some of the films with the highest gross included Star Wars: Episode VII - The Force Awakens, Avengers: Infinity War and The Lion King.

## Finding Correlations in the Data 

* I looked into the budget and the gross to find whether there was any correlation between the two. To quickly compare this, I visualised a scatterplot with budget vs gross.
![download](https://github.com/MariaTayo/Movie-Correlation-with-Python/assets/117232459/e5b2743c-6a69-46a1-8795-c22760f25c43)

Source: This dataset was downloaded from https://www.kaggle.com/datasets/danielgrijalvas/movies 
(scraped from IMDb)

