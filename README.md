# Amazon product recommendation system project
This repository presents a notebook where we are  building a recommendation system to recommend products to customers based on their previous ratings for other products. 
This recommender uses a collection of labeled data of Amazon reviews of products. The goal of this project is to extract meaningful insights from the data and build a recommendation system that helps in recommending products to online consumers.

# Data set 
The dataset contains 7,824,482 user ID (user_id), product ID (prod_id) and ratings observations.
For computational reasons and to ensure that each product and user had enough interaction for the model to identify trends we have filtered users who have given at least 50 ratings, and the products that have at least 5 ratings.

# Tested models
* Rank Based Recommendation System
* Collaborative Filtering Recommendation System both user-user and item-item
* Model-Based Collaborative Filtering - Matrix Factorization

# Takeaway results
* The results show that every models had F1-score over 0.8 which is really good.
* The matrix decomposition did not encounter the lack of neighbor issues that the optimized item-item or user-user Collaborative Filtering Recommendation System encountered. If we aim for a **robust system the matrix decomposition is therefore recommendable**.
* The optimised item-item Collaborative Filtering Recommendation System had the highest score so if we look for **absolute performance the item-item Collaborative Filtering Recommendation System is a good recommendation**
While this work did not look at timestep we recommend using extending timestamp to the study. User shopping tastes evolves through time (example: people buy more christmas decoration in November December to prepare Christmas than the rest of the year)
