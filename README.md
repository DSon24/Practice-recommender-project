# MovieLens Recommender System Practice

This is a **tutorial-based learning project** following the [Building a MovieLens Recommender System workshop](https://www.youtube.com/watch?v=XfAe-HLysOM&t=3257s). The notebook explores movie ratings and builds a simple Bayesian-adjusted movie ranking. It is practice with the early stages of a recommender workflow, not a finished personalized recommendation model.

## What I implemented

The completed notebook is [`Code/practice recommender.ipynb`](Code/practice%20recommender.ipynb). It:

1. Loads `ratings.csv` and `movies.csv` from the **MovieLens latest-small** dataset and explores rating counts, rating distributions, and frequently rated movies.
2. Shows why a movie with a perfect average from only two ratings can be misleading. In the saved run, *Lamerica (1994)* has two 5-star ratings.
3. Computes a Bayesian-adjusted score for every movie using the overall movie-average rating and the average number of ratings as a prior. The example above moves from a raw 5.0 average to an adjusted **3.543**.
4. Ranks movies by the adjusted score, then counts and visualizes movie genres.

The saved output reports **100,836 ratings**, **610 users**, and **9,724 rated movies**. This is a non-personalized movie ranking and exploratory analysis. The notebook does not train collaborative filtering, predict user ratings, or evaluate personalized recommendations.

## Run the notebook

1. Download and extract [MovieLens latest-small](https://grouplens.org/datasets/movielens/latest/). This project uses `ratings.csv` and `movies.csv`.
2. Open [`Code/practice recommender.ipynb`](Code/practice%20recommender.ipynb) in Jupyter. In its first data-loading cell, replace the author's `C:\Users\songu\Downloads\...` paths with the locations of your two CSV files.
3. Install `pandas`, `numpy`, `matplotlib`, `seaborn`, and Jupyter, then run the cells in order.

**Tutorial credit:** [Building a MovieLens Recommender System](https://www.youtube.com/watch?v=XfAe-HLysOM&t=3257s). **Dataset credit:** [GroupLens MovieLens latest-small](https://grouplens.org/datasets/movielens/latest/). The dataset is not included in this repository.
