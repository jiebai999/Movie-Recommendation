# Movie-Recommendation
The object of this project is to use an Alternating Least Squares (ALS) algorithm with Spark APIs to predict the ratings for the movies in MovieLens small dataset
https://grouplens.org/datasets/movielens/latest/
-------------------------------------------------------------------------------------
## Data Analysis, Modeling, Evaluation
1. Conduct exploratory data analysis like split genres into categories, count the number of movies under each category, etc.
2. Build a recommendation model based on historical movie ratings and solve it by matrix factorization and alternating least squares (ALS). 
3. Tune the model parameters through grid search and crossvalidation with the metric root mean square errors (rmse). The optimal model has rmse = 0.64 on the training    dataset and rmse = 0.889 on the test dataset.
4. Recommend 10 movies to some certain users and find top 10 similar movies in terms of some specific movies.
## Notes
*The best model I got has 5 latent factors (hidden features). These features describe a movie in 5 dimensions. Based on the feature, I can define the similarity between movies.