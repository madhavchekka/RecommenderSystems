# Recommender Systems

## Problem Statement:
1. To explore MovieLens dataset with 1M anonymous ratings, 6040 users, and 3900 movies. [MovieLens Dataset](https://grouplens.org/datasets/movielens/1m/)  
2. To explore different recommendation techniques like Collaborative Filtering, Matrix Factorization to recommend personalized content to users 


## Steps Performed: [Link to Code](https://github.com/madhavchekka/RecommenderSystems/blob/master/MovieLens%20Recommender%20Systems.ipynb) 
1. Data Pre-processing - Merging the datasets (ratings, users, and movies)
2. Exploratory Data Analysis
3. Feature Engineering 
4. Univariate, Bivariate, and Multivariate Analysis
5. Collaborative Filtering - Represent Movies & Users as vectors
   -   Custom **Recommender** Functions to perform Item-Item Similarity
       -   Pearson Correlation
       -   Cosine Similarity
6. Matrix Factorization
   -   Utilize Surprise Library to generate Embeddings via **Support Vector Decomposition** Technique for Movies & Users
   -   Custom **Recommender** Functions to perform Item-Item Similarity using embeddings
       -   Pearson Correlation
       -   Cosine Similarity
    
## Insights:
- There 3883 unique movies & 6040 unique users in the given dataset. Release Year of the movies range from 1919 till 2000
- Majority of ratings are given by college/grad students, followed by executive/managerial occupations. ~70% of the users are Male
- There are 250 or more movies for each year - from years between 1994 till 1999
- From 1994 - 2000, proprotion of Movies with one of the genres as Drama or Comedy are higher
- There are ~ 2000 movies with number of ratings between 0 to ~150. Only small proportion of movies have higher and higher count of ratings. Right skewed distribution
- Majority of movies fall into Drama genre, followed by Comedy, Action, Thriller, and Romance. Median value of average rating of movies is little less than 3.5
- Users between ages of 25-34 are in higher proportion amoung Zee users
- College Students tend to rate more when compared to users from other occupations


## Recommendations:
- Identify movies with mean lower ratings and remove from the platform. Utilize the savings to bring early releases to the platform
- Pick recommendations from different algorithms used and see which method's recommendations yield in higher Precision@k to improve the recommendations further
- Gender of users is imbalanced. More content catered to female users might increase female users
- Targeted content for Females, users of retirement age groups would improve the subscriber count
- More datapoints like No of times watched, amount of time watched on the user would help in better recommendations
- Consider UI improvements - to make it easier for users to rate the movies
- Based on the resources, NNs can be used to personalize recommendations as well


