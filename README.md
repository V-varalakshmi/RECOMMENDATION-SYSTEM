# RECOMMENDATION-SYSTEM

*COMPANY*:CODETECH IT SOLUTIONS

*NAME*:RAVAVARAPU VENKATA VARALAKSHMI DEVI

*INTERN ID*:CT06DL1153

*DOMAIN*:MACHINE LEARNING

*DURATION*:6 WEEKS

*MENTOR*:NEELA SANTOSH

DESCRIPTION:

This project involves building a Recommendation System using Collaborative Filtering techniques, specifically user-based collaborative filtering utilizing cosine similarity. The goal is to suggest personalized recommendations by analyzing user behavior and preferences based on rating data. The dataset used is a large CSV file (large_ratings.csv) containing user_id, item_id, and rating columns. The script begins by loading and displaying the original data using Pandas. It then transforms the raw data into a user-item matrix using the pivot function, which organizes the dataset with users as rows, items as columns, and ratings as values. Missing ratings are filled with zeros, indicating that a user hasn't rated those items yet. This matrix becomes the core input for computing similarities between users, based on how similarly they have rated items.

Next, the script calculates the user similarity matrix using cosine similarity from scikit-learn, which measures the cosine of the angle between user vectors in a high-dimensional space, effectively quantifying how similar users are in their preferences. The result is a symmetric matrix where each entry represents the similarity between two users. The core functionality lies in the recommend_best_item function, which generates personalized item recommendations for a specified user. For a given user_id, the function retrieves that user’s similarity scores with other users and their rating history. It then identifies items that the user has not rated and calculates a weighted average score for each of those items based on the ratings from similar users. The recommendation is determined by selecting the item with the highest predicted score. If the system finds at least one such item, it returns the top recommendation with its predicted rating; otherwise, it notifies that no recommendations are available due to insufficient data.

This project aligns well with the learning goals of the internship by applying real-world data and implementing a collaborative filtering-based recommendation engine. It demonstrates an understanding of user-item interactions, matrix operations, similarity measures, and recommendation logic. Although this script focuses on user-based collaborative filtering, the structure allows future expansion into item-based filtering or matrix factorization methods like Singular Value Decomposition (SVD) for enhanced accuracy and scalability. To meet the internship deliverables, this work can be encapsulated in a Jupyter Notebook or deployed as a simple app interface that takes a user ID and returns item suggestions. Additionally, evaluation metrics like RMSE (Root Mean Squared Error) can be introduced in future iterations to quantitatively assess prediction accuracy. Upon successful completion, a completion certificate will be issued by CODTECH, acknowledging the intern’s effort and understanding of recommendation systems, a valuable skill in domains like e-commerce, media streaming, and personalized marketing.

#OUTPUT:

![Image](https://github.com/user-attachments/assets/8050a8cc-fc15-483c-8a9c-2cb9be9b7acb)

![Image](https://github.com/user-attachments/assets/9191c939-c54e-4698-a4d0-62c7a7780f34)
