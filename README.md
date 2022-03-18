# Movie-Recommendation
The object of this project is to use an Alternating Least Squares (ALS) algorithm with Spark APIs to predict the ratings for the movies based on userID and movieID in MovieLens small dataset
https://grouplens.org/datasets/movielens/latest/
![image](https://user-images.githubusercontent.com/52012182/159020325-125f64ae-8e55-44a9-b79a-be93670c2299.png)
-------------------------------------------------------------------------------------
## Alternating Least Square(ALS) Matrix Factorization in Collaborative Filtering
1. Model learns to factorize rating matrix into user and movie representations, which allows model to predict better personalized movie ratings for users
2. With matrix factorization, less-known movies can have rich latent representations as much as popular movies have, which improves recommender’s ability to recommend less-known movies
![image](https://user-images.githubusercontent.com/52012182/159020782-c5de7fd8-b1ae-4a85-920f-5e0be6c4c180.png)

## Data Analysis, Modeling, Evaluation
1. Conduct exploratory data analysis like split genres into categories, count the number of movies under each category, etc.
2. Build a recommendation model based on historical movie ratings and solve it by matrix factorization and alternating least squares (ALS). 
3. Tune the model parameters through grid search and crossvalidation with the metric root mean square errors (rmse). The optimal model has rmse = 0.64 on the training    dataset and rmse = 0.889 on the test dataset.

![image](https://user-images.githubusercontent.com/52012182/159018592-db1e2daa-a0be-497f-ae98-376ddb4ec6b5.png)

5. Recommend 10 movies to some certain users and find top 10 similar movies in terms of some specific movies.
![image](https://user-images.githubusercontent.com/52012182/159020028-e8875ae6-48e9-4519-9a2e-b97e73d5860b.png)

## Notes
* The best model I got has 5 latent factors (hidden features). These features describe a movie in 5 dimensions. Based on the feature, I can define the similarity between movies.

![image](https://user-images.githubusercontent.com/52012182/159024243-fc3e62d9-7986-4ab2-b62a-a8d893e15d7c.png)
