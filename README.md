In this project, we use a basic collaborative recommendation system only, or more specifically:
•	User-based collaborative filtering (UBCF model): it is based on finding similar users and find the items those users have liked but we haven’t tried yet.
•	Item-based collaborative filtering (IBCF model): in this case, we will find similar products to the one the user has bought, and we will recommend those products that are like those which has ratted as best.

For modeling this project has been used R package “Recommender Lab” and Python’s Natural Language Toolkit (NLTK). The main goal of the recommendation system – recommend top 3 products from Amazon that a person can potentially buy next.

Data

•	The CSV data file was collected from the Kaggle website. 
•	This dataset contains reviews of fine foods from Amazon. 
•	The data spans over a period of more than 10 years, including all ~500,000 reviews up to October 2012. 
•	Reviews include product and user information, ratings, and a plain text review. It also includes reviews from all other Amazon categories.
•	Link to the Dataset: https://www.kaggle.com/snap/amazon-fine-food-reviews

Key metric: precision - 80%. 

In this project we used simple recommender systems that don’t use the whole potential of the text data that we have - mostly rely on reviews’ score or reviews’ summary. Even though these models showed pretty good results they are far from perfect recommendation system: work good with people who is actively reviewing and scoring products. These models predict good for no more than 5 items (used for prediction of top 3 items). Surprisingly, Amazon still uses this collaborative filtering recommendation model, even though they test deep learning models constantly.

As a next step we need to implement BERT Embedding recommender system: feature extraction techniques and hybrid deep learning methods for sentiment analysis exploiting the advantages of BERT, to incorporate sentiments into recommendation methods as additional feedback and thus improve the performance and the reliability of recommender systems. However, it will require update data and use not only ProductId, but the names of the items and short description of each item. 

