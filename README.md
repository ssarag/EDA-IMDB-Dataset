# Exploratory Data Analysis on IBDM dataset. 

# Objectives for the Analysis
1. Indentify Trends in the dataset and come up with a suggestion of a movie which will give good money returns and profit.
2. Test the results by carrying out hypothesis testing 

# Dataset

The dataset utilized here is taken from IMDB movie review dataset. This dataset contains information such as Movie Name, Budget, Actors, Producers, Directors, Language, Profit, Duration of the movie, etc. The dataset is split into two parts, Train and Test with the ratio 70:30. We will be using the train dataset for our EDA and test the hypothesis on test dataset.

# Hypothesis 

Null Hypothesis(H0): The movies with greater IMDB score generate good money returns and profit. 

Alternate Hypothesis(H1): The greater IMDB score does not gaurantee profits of the movie

For doing the hypothesis I will be doing two sided T test

taking p value = 0.05.

If the value of the T-test is less than the P value we will reject the hypothesis.


# Analysis

The first step in the EDA is to split the dataset into train and test (70:30) and check for null entries. The null entries for numerical data were repleced by Imputing the null entries with the median of each column. 


![image](https://user-images.githubusercontent.com/103538049/200134439-28c9166c-b122-474d-9762-f307e9814381.png)



In the next step, we are sorting the mean imdb score and budget across films by genre.Here, we have set a minimum imdb score and filter according to that. We are interested only in high scores so we are only looking at films with good ratings.


![image](https://user-images.githubusercontent.com/103538049/200134827-a0ea116e-a57b-4530-ad21-03d50dd2e809.png)


Next, we are calculating the profit of the movies. After calculating the profit I will use it to calculate the profit each actor has earned from the total number of likes on facebook page. This will give us an idea if the success of the movie depends on the popularity of the actor. As we can see from the below graph there are actors with less fan follow base but still their movies have earned profits and movies of the actors with more likes on facebook does not have significant amount of profit. So the idea that the success of the movie depends on actors facebook likes is not true here


![image](https://user-images.githubusercontent.com/103538049/200134918-8bbf43a6-0a77-40bd-b27b-e6086855760b.png)


Plotting a graph of the profit value of each actor and imdb score to see if the profits earned by the actor suppurts high rates on IMDB. As we can see from the graph the idea holds true. That means if the IMDB score and actor's individual profit are related to each other.


![image](https://user-images.githubusercontent.com/103538049/200134982-adcb3445-ac0f-41d5-8419-799b21bd9d54.png)



Checking which genres have good IMDB scores aslo their budget and profit. The top 5 genres are showed below.

![image](https://user-images.githubusercontent.com/103538049/200135031-2004f3b5-8644-4bc7-8652-c8014e97b277.png)


Higher Budget gives higher profit

![image](https://user-images.githubusercontent.com/103538049/200135064-76da457a-b836-4f34-8be3-6ce76a814f76.png)


Movie Duration 

![image](https://user-images.githubusercontent.com/103538049/200135096-8e9089fb-1925-4687-9d20-10186e2fdb45.png)


Bell curve to see the probability distribution of Budget, profit and gross.


![image](https://user-images.githubusercontent.com/103538049/200135126-98e82078-4359-4308-8d9f-6915f0f06b79.png)

The most popular co-actors, directors and producers with IMDB rating greater than 8. 

![image](https://user-images.githubusercontent.com/103538049/200135178-6460eccf-42fa-4485-9324-503d14b713c8.png)


# Summary 


We examined the IMDB data to look for appropriate movies and find a trend in the movies for analyzing whcih type of movie should be produced for earing maximum profits and success. For analyzing the data we divided the data into 2 parts train and test. The data analysis was done on train data set and the testing was done on test data set.


Here we examined whether there are films with specific genre that get more profit and found that Sci-fi, Drama, Thriller have more number of votes from users and their budget is also less with good IMDB rating.

We also checked if there is any relation between the cast of the movie and profit. Below is the observation :
1. Searched for trios of the actors who have worked toghter more frequently in a movie and the movie has earned profits with good IMDB rating and found that there are few examples of such cases where the actors who have worked toghter have earned more profits. 
2. Looked for the total likes of the actors and director and the observation was that the actors with more number of likes earned more profits in the movie

# Conclusion

Bssed on the above data analysis and hypothesis it is recommend to produce a movie with actors who have worked togheter earlier and have good IMDB rating. The movie should be made on Drama|Thriller genre as it is one of popular genre with good ratings. The movie can be released in USA as most popular movies have have been from USA with English language.
