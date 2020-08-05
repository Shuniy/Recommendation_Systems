# Recommendation Systems

We will be custom implementing 4 types of Recommendation Systems:
- Rank Based Recommendations
- User-User based Recommendations
- Content Based Recommendations
- Matrix Factorization
  
[Implementation can be found here](https://github.com/ZippySphinx/Recommendation_Systems/blob/master/Recommendation_Systems.ipynb)

#### Rank Based Recommendations
>Rank based Recommendations are derived from Knowledge based Recommendations. Knowledge based recommendations are the top recommendations according to their ratings. Rank based recommendations uses knowledge based recommendations but with some filters as per the user.

#### User-User Based Collaborative Filtering
>- Collaborative filtering is a method of making recommendations based only on the interactions between users and items. 
>- In User-User recommendations it works with interaction between user and item but in this recommendations are made with the similarity between users. We will be using cosine method of finding similarity and then taking the items from the most similar users.

#### Content Based Recommendations
>- Another popular technique for making recommendations is called content based recommendations. In this recommendation technique, we use information that is known about the user or item to make recommendations. This method of making recommendations is particularly useful when we do not have a lot of user-item connections available in our dataset.
>- It might be the case that content based and collaborative filtering based techniques come up with similar recommendations, but the methods by which data scientists approach these recommendations are very different. In collaborative filtering, you are using the connections of users and items (as you did before). In content based techniques, you are using information about the users and items, but not connections (hence the usefulness when you do not have a lot of internal data already available to use).

#### Matrix Factorization
>- We will be suing SVD (Singular Value Decomposition).
>- In order to implement SVD for many recommendation engines, we will need to use a slightly modified approach known as FunkSVD. This approach proved to work incredibly well during the Netflix competition, and therefore, it is one of the most popular recommendation approaches in use today.
>- When performing SVD, we create a matrix of users by items (or customers by movies in our specific example), with user ratings for each item scattered throughout the matrix.
>- You can see that this matrix doesn't have any specific information about the users or items. Rather, it just holds the ratings that each user gave to each item. Using SVD on this matrix, we can find latent features related to the movies and customers. This is amazing because the dataset doesn't contain any information about the customers or movies!

### Packages Used
- scikit-learn
- pandas
- numpy
- matplotlib
- nltk
- pickle