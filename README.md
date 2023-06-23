# Recommender_Systems
This project focuses on building accurate recommender systems using deep learning. It includes algorithms like matrix factorization, SVD, and deep neural networks, along with practical aspects like handling big data. Valuable for developers and data scientists in the field.

Focus: This GitHub repository is dedicated to a project on building and implementing recommender systems using deep learning techniques.

Goal: The project aims to provide accurate recommendations to users based on their preferences and behavior.

Algorithms: The repository includes code and resources for implementing various algorithms like matrix factorization, SVD, and deep neural networks.

Practical aspects: It covers practical aspects such as handling big data with Spark and AWS EC2 clusters.

Benefits: Exploring this repository offers insights and practical knowledge in recommender systems, data science, machine learning, and AI.

Audience: It serves as a valuable resource for developers and data scientists interested in building advanced recommendation systems.

Cutting-edge techniques: The repository focuses on using state-of-the-art techniques to develop advanced recommendation systems.

![image](https://github.com/burzin25/Recommender_Systems/assets/84149050/316f11e1-cca2-43b7-ae60-9155676e0c61)

# What Is Recommendation System?
A recommendation system is a type of algorithm that predicts what rating or preference a user might have for an item. It's like a smart tool that suggests things you might like. For example, on Netflix, it helps you decide which movie to watch, on e-commerce websites it suggests products to buy, and on Kindle, it recommends books to read.

# Content Based Filtering

Tagging: Products/items are tagged using keywords or attributes that describe their content. For example, in a movie recommendation system, movies are associated with genres as tags.

Initial Recommendations: When a new user, let's say User A, arrives, the system may recommend popular items or ask the user to fill out a form to gather some initial information.

User Ratings: Over time, as User A interacts with the system, they may provide ratings to movies based on their preferences. For example, they might rate action movies highly and give poor ratings to anime movies.

Content-based Recommendations: Using the information gathered, the system recommends items to User A based on their preferences and the content (tags) of the items. In this case, the system would recommend action movies to User A.

Limitations: It's important to note that the system may not have a complete understanding of User A's preferences. For example, User A might have disliked a particular anime movie due to reasons like acting or story, rather than disliking the entire anime genre. The system needs more data to make accurate recommendations.

Advantages of content-based filtering:

Recommendations are specific to each user, as the model doesn't require data from other users.
It can easily scale to a large number of users.
The model can capture the specific interests of a user and recommend items that align with their unique preferences.
Disadvantages of content-based filtering:

Hand-engineering the feature representation of items requires domain knowledge.
The model can only recommend items based on a user's existing interests and has limited ability to expand on their preferences or suggest entirely new items.

# Collaborative Filtering

Collaborative filtering is a way to recommend new things to users based on the interests and preferences of other similar users. For example, when we shop on Amazon, it suggests new products by saying "Customers who bought this also bought...".

There are two types of collaborative filtering:

User-Based Collaborative Filtering: This method looks at the ratings and preferences of similar users to make recommendations. If users A and C have similar tastes, and user A liked certain items, user C might be recommended those items too.

![image](https://github.com/burzin25/Recommender_Systems/assets/84149050/70939bf4-8750-4791-abc0-016a61f07317)


Item-Based Collaborative Filtering: This approach predicts ratings based on the user's own ratings on similar items. If children A and B both liked watermelon and grapes, and child C liked watermelon, they might be recommended grapes.

![image](https://github.com/burzin25/Recommender_Systems/assets/84149050/570901cf-893f-490d-b5ee-5da7890de0fc)


Advantages of collaborative filtering:

It works well even with small amounts of data.
It helps users discover new interests based on the preferences of similar users.
It doesn't require domain knowledge about the items.
Disadvantages of collaborative filtering:

It cannot handle new items that have not been previously rated by users (known as the "Cold Start Problem").
Side features like actor names or releasing years may not have much importance in the recommendations.

# When deciding between user-based and item-based collaborative filtering, you can consider the number of items and users in your system.

User-Based Collaborative Filtering: If the number of items is greater than the number of users, it's more efficient to use user-based collaborative filtering. This approach reduces computational power by focusing on similarities between users rather than comparing a large number of items.

Item-Based Collaborative Filtering: If the number of users is greater than the number of items, it's preferable to use item-based collaborative filtering. This method takes advantage of the larger user base to find similarities in item preferences, as there are fewer items to compare.

For example, Amazon has millions of products available for sale but billions of customers. Therefore, Amazon uses item-based collaborative filtering because the number of products is significantly smaller compared to the number of customers, making it more practical to analyze item similarities.

By considering the ratio of items to users, you can choose the appropriate approach to optimize the performance of your collaborative filtering system.
