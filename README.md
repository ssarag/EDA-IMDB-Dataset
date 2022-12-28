# EXPLORATORY DATA ANALYSIS ON IMDB DATASET

In this project I will be doing analysis of IMDB dataset obtained from kagggle. Few of the business questions that I am going to explore are as below.




1. What are the top rated movies?
2. Which genre of the movies is mostly liked by the audience?
3. Which movies have the highest gross?
4. Do the movies with highest IMDB rating earn highest gross always?
5. What is the trend analysis of the movie genre preferences by the audience?
6. Who are the top rated direnctors and actors?
7. What runtime is good to get a good IMDB rating and gross?
8. For a movie to be sucessful, design a plan which should include Genre, director, actors and runtime of the movie. 


# The dataset contains the following columns. 

1. Poster Link - Link of the movie posters.
2. Series_Title - Name of the movie.
3. Certificate of the movie.
4. Runtime - Time of the movie in minutes.
5. Genre - Genre of the movie.
6. IMDB_Rating.
7. Overview - A short overview of the movie in few sentences.
8. Meta score
9. Director name
10. Names of the actors (4 maximum)
11. Gross
12. No of votes


![image](https://user-images.githubusercontent.com/103538049/209874369-5c708c2e-0dc2-477c-8664-b5f50d1cc403.png)

Next, I am Checking for null entries in the data. As it can be seen from the result there are few null entries in colums **'Certificate', 'Gross' and 'Meta score'**, I am using pandas fillna() method to replace the NaN values with the mean of the respective columns.

# Analysis

# 1.What are the top rated movies? 

To check the movies with highest rating, I am groping the movies with rating greater than 8 and theri genre.Few of the classic high rated movies are as below.

![image](https://user-images.githubusercontent.com/103538049/209874509-35451d0a-348c-48e4-88e3-84eb4e06f7d4.png)


# 2. Which genre of the movies is mostly liked by the audience?

Here, the genre from top rated movies is selected. The movies range from the year 1920 to the year 2020. The below pie chart shows the all time favourite genre by the audience. The most watched genre is Crime-Drama. In the further parts we will also be doing a trend analysis of the genre to get a clear picture of the latest genre loved by the audience.

![image](https://user-images.githubusercontent.com/103538049/209874574-05e7399e-b9c9-4454-b7b5-1c99a86ef461.png)

