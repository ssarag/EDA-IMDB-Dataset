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


# 3. Movies with highest Meta score and their IMDB rating

From the dataset we can see that the highest meta score of the movies is 100. Even tough few movies have high meta score, theri rating less as compared to the movies with less meta score and high rating. This suggests that Meta score is not a reliable factor to decide the sucess of the movies.


![image](https://user-images.githubusercontent.com/103538049/209874746-7952f439-86e1-4e9a-9a1b-9caec84c1fbe.png)


# 4. Average time duration of the movies

Next, I checked what is the average runtime of the movies from the year 1920 to the year 2020. In the next part, I will also be exploring the runtime of the movies accoring to theri rating.As we can see from the histogram below, the average runtime of the movies is between 100 mins - 150 mins.

![image](https://user-images.githubusercontent.com/103538049/209874865-f66710d4-9d78-4231-a38f-97624af97267.png)

# 5. Certificates of the top rated Movies
Next, I explored the top rated movies and their certificates. As it can be seen from the below pie chart, most of the top rated movies are "A" certified or "U" certified

![image](https://user-images.githubusercontent.com/103538049/209874945-55ea8e30-69a1-470c-a0b4-91ecb84400d8.png)


# 6. Which are the highest grossing movies

![image](https://user-images.githubusercontent.com/103538049/209875028-dc559168-a929-4123-86cf-09c1ae5d802a.png)
![image](https://user-images.githubusercontent.com/103538049/209875059-bf767a8b-2056-4e5b-95f9-86452e47ed8c.png)



We can see from the above figures that movies with ratings greater than 8 have the closer averege gross, and only a few movies have made exceptional gross. In the next section I am analyzing the movies with highest gross.


![image](https://user-images.githubusercontent.com/103538049/209875134-d7fface5-7a5c-472f-b686-a8bb53b383aa.png)

From the above result, it is clear that even tough some of the movies do not have the best IMDB score, they have still managed to generate maximum gross. Movies like Star Wars, Avatar, Titanic, Incredibles are among the top gross generating movies. In the next part, I am exploring the genre of the movies wih highest gross and as it can be seen from the pie chart, the genre 'Action, Adventure,Sci-Fi' generates more gross as compred to the genre 'Crime, Drama' which is among the highest IMDB Rating movies.

![image](https://user-images.githubusercontent.com/103538049/209875213-29f3a0e0-96d7-424e-a228-c92144baf7cd.png)



