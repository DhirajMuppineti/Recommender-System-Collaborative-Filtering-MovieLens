# Recommendation System

When you go to an e-commerce platform, one of the most important factors that induces you to make the actual purchase is how quickly are you able to locate the item you want to buy. One way in which ecommerce platforms achieve is through recommendation systems (also known as recommender systems), e.g. the ‘customers who bought this item also bought…’ section on Amazon. Almost all e-commerce platforms as well as movie & song streaming platforms like Amazon prime, Spotify, Netflix use a variation of recommendation system algorithm. The idea is to improve the user experience. There is an unwritten rule in any business - more happy is your customer, more is your profits.

## Collaborative filtering

The one of the extremely popular technique is __collaborative filtering__. The basic idea of collaborative filters is that similar users tend to like similar items and it is based on the assumption that, if some users have had similar interests in the past, they will also have similar tastes in the future too. In collaborative systems, the main advantage is that you do not need to know the content in detail. Amazon’s product ‘Customers who bought this item also bought…’ is a popular example of collaborative filtering. When you buy Inferno by Dan Brown, it recommends other books which were bought by other people who also bought Inferno. In this case, the system may not even care about the genre or the price of the books being recommended; it simply recommends them to you because other people similar to you bought them.

#### User-based Collaborative Filtering

In user-based collaborative filtering, you try to find users who have similar tastes and preferences, based on the past ratings they have given to the same items. The similarity between the users is represented in terms of correlation or cosine similarity. Finally, you can use the weighted sum of the ratings provided by like-minded users for an item to predict what rating may be provided by a user.

#### Item-based Collaborative Filtering

Another extremely successful type of collaborative filtering algorithm is item-based collaborative filtering. Item-based systems are heavily used by companies such as Amazon and various movie recommendation sites. In user-based collaborative filters, you measure the similarity between users. The basic idea is that similar users are likely have similar tastes. In contrast, item-based systems calculate the similarity between various items or products. Next the rating that a particular user will give on a given item is predicted by taking weighted sum of ratings provided by the user on different items that are similar to the given item. 

## About MovieLens dataset

This dataset (ml-latest-small) describes 5-star rating and free-text tagging activity from MovieLens, a movie recommendation service. It contains 100836 ratings and 3683 tag applications across 9742 movies. These data were created by 610 users between March 29, 1996 and September 24, 2018.

Credits: F. Maxwell Harper and Joseph A. Konstan. 2015. The MovieLens Datasets: History and Context. ACM Transactions on Interactive Intelligent Systems (TiiS) 5, 4: 19:1–19:19. https://doi.org/10.1145/2827872

#### Ratings Data File Structure (ratings.csv)

  - All ratings are contained in the file ratings.csv. Each line of this file after the header row represents one rating of one movie by one user, and has the following format: userId,movieId,rating,timestamp

  - The lines within this file are ordered first by userId, then, within user, by movieId.

  - Ratings are made on a 5-star scale, with half-star increments (0.5 stars - 5.0 stars).

  - Timestamps represent seconds since midnight Coordinated Universal Time (UTC) of January 1, 1970.

Link for MovieLens dataset: https://grouplens.org/datasets/movielens/
(The dataset used in this project is in ml-latest-small.zip)
