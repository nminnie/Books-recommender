# Books recommender system
To see the full notebook and get your own book recommendations, visit [this notebook.](https://nbviewer.jupyter.org/github/nminnie/Books-recommender/blob/master/recommender_model.ipynb)

## The Datasets¶
We have two datasets:

* books.csv contains information for 10,000 books, such as ISBN, authors, title, year, etc.
* ratings.csv is a collection of nearly 6 million user ratings for these books, ranging from 1 to 5 stars

## The Approach
The recommendation approach we will use is collaborative filtering, which make recommendations for a user according to how other users consume or rate items. The idea is that if two users consume or rate items in a similar way, then they probably like the same items.

## Feature Engineering
To employ the approach above, we need to construct a matrix of users and their books ratings. This users-ratings matrix will be sparse, as there are many books in the dataset than what an average user reads or rates, but we can compress this matrix before training the model.

## The Algorithm
We used an unsupervised version k-Nearest Neighbors, with cosine similarity as the distance metric. Since this is an unsupervised learning task, there is so measure of accuracy score so we cannot use cross validation and require human judgement to evaluate how well the model recommends books.
