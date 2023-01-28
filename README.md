# Movie-Recommendation-System-Using-Python-and-Spark
#### I dig deep into collaberative recommendation engine by using Spark, Python, Pandas and scikit learn to give recommendation with user based movie recommendation with a scalable matrix vectorizer technique.
### Step1 
First ingested datasets using spark Dataframes, namely movies and ratings and conduct a number of data explorations on these data to get some basic information, such as number of users, number of movies, number of ratings per users and per movies respectively, and distribution of movies on different genres.
#### Movie Dataset Sample
![image](https://user-images.githubusercontent.com/69915064/215246475-1fd1f3c9-64b5-4e55-b685-88b97919ea6d.png)
#### Ratings Dataset Sample
![image](https://user-images.githubusercontent.com/69915064/215247063-7c20ee51-debf-4d30-8445-80484896e4bd.png)

### Step2
After Ingesting Dataset into Spark Dataframe We cleaned data using Python Regex to remove special Characters(chars like !,@,#,$,%...etc) from title of the movie.
##### As you can see in below dataset there is paranthases and comma(,) available in movie titles which makes it difficult to search movie by its name/title
![image](https://user-images.githubusercontent.com/69915064/215247853-43e41563-0a8d-4a96-a787-1183e6d39268.png)
##### As you can see after cleaning there is no paranthases or any other special chars available in the title column
![image](https://user-images.githubusercontent.com/69915064/215247993-58e0fdf7-39d7-47a0-8017-19ac064cec7b.png)

### Step 3
![image](https://user-images.githubusercontent.com/69915064/215248315-ecce7657-5bc2-4f00-9121-1ff44d63cadd.png)

Then we are creating search engine using scikitlearn library to vectorize our movie dataset to make it ready for search engine

#### Finaly...
![image](https://user-images.githubusercontent.com/69915064/215248272-3484a328-e19b-4f3f-b027-24dc24b8997b.png)

Then we have created Recommendation Engine using collaborative filtering where if we enter name of any movie which we likes then engine will recommend to us some top movies which we me may like to watch

![image](https://user-images.githubusercontent.com/69915064/215248175-b324c724-d660-4680-b2c8-0f3a18fa3f2e.png)
![image](https://user-images.githubusercontent.com/69915064/215248180-fc9164e2-78a3-4b78-8937-fcbb11f35a9f.png)



