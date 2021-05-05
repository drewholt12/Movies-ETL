# Movies-ETL


# Purpose
Amazing Prime employees are having a hackathon event to analyze data about movies for decisions about their streaming service.  Their hope is to develop an algorithm to predict popular, low budget movies that will become popular to bring business to their service.   Utilizing data from Wikipedia from 1990 to 2018 and MovieLens data curated  by Grouplens housed on the website Kaggle, the team hopes to find solutions to the question.  

# Overview
To extract, transform, and load data to a database for analysis.
Analysis requirements:
  1. write a function to extract and transform data from 3 data sources- Wikipedia, Kaggle, and ratings
  2. load transformed data into a database

# Resources
## Source data:
    1.movies_metadata.csv
    2.ratings.csv
    3.wikipedia-movies.json

## Software/dependencies
    1. Python
    2. Pandas
    3. Numpy
    4. SQLAlchemy
    5. psycopg2
    6. PostgreSQL/PGAdmin


# Results
Data sets were extracted and inspected  through creation of a function.  Data sets were cleaned for null values and unnecessary columns.  Columns with incorrect headings were renamed or data moved to appropriate columns using IMDB ID information.  Comparison of the data sets for redundant or inconsistent data was performed.  Data sets were merged with the most complete data, where columns were renamed to better describe their contents.  The result is 2 tables in the database for which the hackathon participants will utilize for further analysis.  One for movie titles with other information including the average rating, budget, income, producer, actors, etc., and one table for movie ratings that focuses on the individual ratings for each movie.  Total row contents of the movie table is 6052, where the ratings table has 26,024,289 rows. 

Movie table
![movies_query](https://user-images.githubusercontent.com/79231355/117210322-21a7c780-adbd-11eb-8b1b-f3ed7c8b79f3.png)

Ratings table
![ratings_query](https://user-images.githubusercontent.com/79231355/117210348-28ced580-adbd-11eb-862e-e94e2dbc7539.png)
