# MovieRecommendationsSystem
Abstract:
This paper reports our experience in building a movie recommendation system. We have used the MovieLens dataset containing several movies and their respective genres and ratings. We have used varied prediction methods and displayed the recommendations obtained from them in this report. 
1. Introduction:

1a. Problem Statement:
The problem requires us to recommend a set of movies to a particular user by filtering the given dataset based on the information provided by the user. This requires us to take into consideration the past engagement of the user as well as knowledge about their likes and dislikes.

1b. The Data:
The dataset comprises 4 separate files. They are:
Movies.csv: contains MovieId, Title, Genres and is of size (9742,3)
Links.csv: contains MovieId, IMDBId, TMDBId and is of size (9742,3)
Ratings.csv: contains UserId, MovieId, Rating, Timestamp and is of size (100836,4)
Tags.csv: contains UserId, MovieId, Tag, Timestamp and is of size (3683,4)

2. Methodology:

2a. Overview:
The various concepts used in our implementation are:
1. Correlation 
2. Matrix Factorisation using Stochastic Gradient Descent
3. Collaborative Filtering using KNN
4. Natural Language Processing

2b. Pre-processing and Visualizing the data:
The datasets were merged several times to suit the particular model. Some of these merged datasets include genre_df, df, user_ratings_df, final_dataset,movie_idx, complete_df, merge_dataset, etc. All the NaN values in the numeric columns were filled with 0 as and when required by the models. 
We also used NLP to process the tags of the movies. To do this, we removed the special characters and one and two-letter words from the data. 
