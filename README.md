### **Project: Amazon Product Recommendation System**

Welcome to the project on Recommendation Systems. We will work with the Amazon product reviews dataset for this project. The dataset contains ratings of different electronic products. It does not include information about the products or reviews to avoid bias while building the model.

--------------
## **Context:**
--------------

Today, information is growing exponentially with volume, velocity and variety throughout the globe. This has lead to information overload, and too many choices for the consumer of any business. It represents a real dilemma for these consumers and they often turn to denial. Recommender Systems are one of the best tools that help recommending products to consumers while they are browsing online. Providing personalized recommendations which is most relevant for the user is what's most likely to keep them engaged and help business.

E-commerce websites like Amazon, Walmart, Target and Etsy use different recommendation models to provide personalized suggestions to different users. These companies spend millions of dollars to come up with algorithmic techniques that can provide personalized recommendations to their users.

Amazon, for example, is well-known for its accurate selection of recommendations in its online site. Amazon's recommendation system is capable of intelligently analyzing and predicting customers' shopping preferences in order to offer them a list of recommended products. Amazon's recommendation algorithm is therefore a key element in using AI to improve the personalization of its website. For example, one of the baseline recommendation models that Amazon uses is item-to-item collaborative filtering, which scales to massive data sets and produces high-quality recommendations in real-time.

----------------
## **Objective:**
----------------

You are a Data Science Manager at Amazon, and have been given the task of building a recommendation system to recommend products to customers based on their previous ratings for other products. You have a collection of labeled data of Amazon reviews of products. The goal is to extract meaningful insights from the data and build a recommendation system that helps in recommending products to online consumers.


### Conclusions:
We built recommendation systems using four different algorithms. They are as follows:
1.  Rank-based using averages
2.  User-User similarity-based collaborative filtering
3.  Item-Item similarity-based collaborative filtering
4.  Model-based collaborative filtering (matrix factorization)



- The **surprise** library was used to demonstrate**"user-user similarity-based collaborative filtering," "item-item similarity-based collaborative filtering," and "model-based collaborative filtering (matrix factorization)"** algorithms. For these algorithms, grid search cross-validation is used to find the optimal hyperparameters for the data, and related predictions are created using the optimal hyperparameters.
- **For performance evaluation** of these models **precision@k and recall@k** are used. Using these two metrics, the **F_1 score** is calculated for each working model.

**Findings:**
- Overall, the **Model-based collaborative filtering (matrix factorization) recommendation system has given the best performance in terms of RMSE (the lowest)  and F1-Score  (only 0.001 lower than the user-user one) .**
- We can try to further improve the performance of these models using hyperparameter tuning.
- Due to sparse data, sometimes the rating preditions are kind of unstable. We may reduce the value of k or implement different algorithm to solve this problem.
- We can also combine different recommendation techniques to build hybrid recommendation systems.