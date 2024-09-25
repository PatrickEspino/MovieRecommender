# Movie Recommender System using PySpark

This project utilzies the [MovieLens](https://grouplens.org/datasets/movielens/) dataset, provided by GroupLens.

This repository contains a Movie Recommender System project imlemented used Apache Spark, focusing on collaborative filtering. The system leverages the Alternating Least Squares (ALS) algorithm to recommend movies based on user preferences and ratings. Data analysis and visualizations are provided using Spark SQL and Matplotlib to explore trends in movie ratings, genres, and release years.

## Project Overview

The primary objective ofc this project is to build a robust recommendation system that predicts user preferences for movies they have not rated yet. This is achieved through collaborative filtering using the ALS algorithm, which factors in both user-item interactions and hidden patterns in the data.

Additionally, the project includes a series of exploratory data analyses to extract insights about movie ratings, genre popularity, and yearly trends in movie releases.

## Features

**1. Data Exploration and Visualizations**
    * Distribution of user ratings
    * Average ratings per genre
    * Number of ratings and movies for each genre
    * Trends in movie releases and ratings across the years

**2. Collaborative Filtering with ALS**
    * **Algorithm**: Alternating Least Squares
    * **Train-Test Split**: 80% training, 20% test data
    * **Hyperparameters**: The model uses a rank of 10, and a regularization parameter of 0.1
    * **Performance Evaluation**: Root Mean Squared Error (RMSE) is used to assess model accuracy
    
**3. Model Tuning**
    * Utilizes a grid of hyperparameters and tested each combination to select best model
    * Cross-validation to fine-tune the ALS model's hyperparameters ensures the model generalizes well to unseen data
    * Tests different strategies for handling missing values, such as filling with average values vs. dropping them entirely

## Insights
* **Distribution of Ratings:** Most users tend to give 3 or 4 stars, indicating a generally positive but moderate sentiment.
* **Genre Ratings:** Some genres like "War," "Crime," and "Western" tend to receive higher ratings than others, which can guide genre-based recommendations.
* **Trends in Ratings:** There is a noticeable drop in the average ratings of movies released between 1960 and 2000, stabilizing post-2000.
* **Movie Popularity Over Time:** The number of movies produced annually has grown exponentially post-2000, suggesting an increase in demand and production within the industry.

