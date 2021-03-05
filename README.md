# Collaborative-Filtering-Recommender-System

![](https://images.unsplash.com/photo-1560169897-fc0cdbdfa4d5?ixlib=rb-1.2.1&ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&auto=format&fit=crop&w=2552&q=80)


in the last notebook we have created a content-based recommender system to recommend similar movies to the user. one of the disadvantages of that algorithm it will always recommend content based on the user  already  watched and does not let him discover new content, also it might misunderstand what the user likes. in this notebook, we will work with a collaborative filtering algorithm.

## What is Collaborative Filtering means?
collaborative filtering recommends a list of movies based on people who like the same things as you, but who also like something that you haven’t yet consumed. its focus on the relationship between users and items. The similarity of items is determined by the similarity of the ratings of those items by the users who have rated both items.
There are two types of Collaborative Filtering:
1.User-based, which measures the similarity between target users and other users. 
2.Item-based, which measures the similarity between the items that target users rate or interact with and other items.

in this notebook we will work with the user based recommendation technique as following:
1.import the data and split it into training and testing data.
2.find 20 nearest neighbors using cosine metric.
3.collect the movies watched by the neighbors and not watched yet from the target user.
4.calculate user predicted ratings.
5.create recommedations withthe top 20 predicted movies.
