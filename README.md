
# Validating Fandango Movie Ratings with Machine Learning

## Overview

Are all **online reviews** really reliable? The majority of people decide to watch movies solely based on such reviews, and it paves the way for movie companies to take advantage of people. In fact, online reviews can easily win the public trust and thus heavily promote certain movies, creating a preconception in people's minds. 

### Goal:

**The goal is to complete the tasks below based on the 538 article and see if we reach a similar conclusion. We will need to use our pandas and visualization skills to determine if Fandango's ratings in 2015 had a bias towards rating movies better to sell more tickets.**


## Business Problem 

Movie producers want to know how audiences will rate new movies before deciding on marketing budgets. By predicting Fandango ratings, producers can make data-driven decisions to maximize box office success.

## Data

This is the data behind the story [Be Suspicious Of Online Movie Ratings, Especially Fandango’s](http://fivethirtyeight.com/features/fandango-movies-ratings/) openly available on 538's Github: https://github.com/fivethirtyeight/data. There are two CSV files, one with Fandango Stars and Displayed Ratings, and the other with aggregate data for movie ratings from other sites, like Metacritic, IMDB, and Rotten Tomatoes.

## Methodology

The methodology involved:

- Exploratory Data Analysis to understand patterns and relationships
- Data cleaning and preprocessing like converting text to numeric features  
- Feature Engineering to derive new features from existing ones
- Train/Validation/Test split to evaluate model on unseen data
- Hyperparameter tuning using GridSearchCV for model optimization
- Building and evaluating various classification models
- Comparing metrics like accuracy, precision, recall to select best model

## Models Used

Models tested include Logistic Regression, Decision Trees, Random Forest, Support Vector Machine and Neural Network. Hyperparameters like number of estimators, max_depth, learning rate were tuned.

## Key Results

The Random Forest model achieved the best validation accuracy of 83% and precision/recall close to 83%. This model is best suited to predict Fandango ratings with high confidence.

## Business Recommendations

Movie producers can use this model to identify movies that may achieve higher ratings and target accordingly with relevant marketing messages for better box office success. Fandango can also use it to prioritize movie listings and recommendations.

## Future Work

Potential improvements include feature engineering from IMDb data, modeling year-wise trends and building separate models by genre tags. Deploying the model as a web service for easy predictions is also recommended.
