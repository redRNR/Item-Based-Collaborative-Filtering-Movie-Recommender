# IBCF Movie Recommender System

## Overview
This project implements an **Item-Based Collaborative Filtering (IBCF)** movie recommendation system using the [MovieLens dataset](https://grouplens.org/datasets/movielens/). The system analyzes user ratings of movies and predicts the top 10 recommendations for a given user. It uses the `recommenderlab` package in R for creating and evaluating the recommendation model.

## Features
1. **Exploratory Data Analysis**: 
   - Generates summary statistics for movies and ratings datasets.
   - Creates a sparse matrix for ratings.
   - Visualizes user and movie similarities using cosine similarity.
   - Plots distribution of rating values and user average ratings.

2. **Collaborative Filtering System**:
   - Builds a recommendation model using cosine similarity.
   - Optimizes the number of nearest neighbors (`k`) to improve recommendations.
   - Evaluates the model using metrics like Root Mean Square Error (RMSE) and Mean Absolute Error (MAE).

3. **Top 10 Recommendations**:
   - Predicts and displays the top 10 recommended movies for a given user based on their rating history.

## Dataset
The project uses a smaller subset of the **MovieLens dataset** containing:
- 100,836 ratings applied to 9,742 movies by 610 users.
- Movies span across 19 genres, with 3,683 unique tags provided by users in reviews.

## Model Evaluation
The IBCF recommendation model was evaluated using:
- **RMSE**: 0.865
- **MAE**: 0.598
- **True Positive Rate (TPR)**: 16.8%
- **False Positive Rate (FPR)**: 1.5%

## Results
The recommendation system demonstrates competitive performance, successfully identifying patterns in user preferences and achieving high accuracy in the generated recommendations.

## Limitations
- **Cold Start Problem**: Users and movies with insufficient data were excluded to ensure reliable predictions.
- **Subset of Dataset**: Due to computing constraints, a smaller subset of the MovieLens dataset was used, limiting prediction accuracy.

## References
- **MovieLens dataset**: [GroupLens Research](https://grouplens.org/datasets/movielens/)
- **Recommender system algorithms**: [Recommenderlab](https://cran.r-project.org/web/packages/recommenderlab/index.html)



