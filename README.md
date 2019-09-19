## Books recommender system
To see the full notebook and get your own book recommendations, visit [this notebook.](https://nbviewer.jupyter.org/github/nminnie/Books-recommender/blob/master/goodreads_recommendations.ipynb)
### The dataset
This dataset contains information (title, author, ISBN) for 10,000 popular books on Goodreads, and almost 6 million ratings (from 1 to 5) from users for these books.
### The recommender model
The algorithm is k-Nearest Neighbors.
The features are stored in a matrix of the users' ratings for the 10,000 books.
The method is collaborative filtering, with the idea that "users that liked this product also liked these products".
