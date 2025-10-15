#  Ecommerce Product Recommendation System

A **machine learning–based recommendation system** that provides personalized product suggestions to users based on their browsing and purchase history. It uses a combination of **rank-based**, **collaborative filtering**, and **model-based** approaches to enhance the shopping experience and boost e-commerce sales.

---

##  Dataset

- **Source:** [Amazon Electronics Ratings Dataset](https://www.kaggle.com/datasets/vibivij/amazon-electronics-rating-datasetrecommendation)
- Each user and product is assigned a **unique ID** (to remove bias).  
- Dataset contains **user ratings** for electronic products.

More datasets available at [UCSD Amazon Data](https://jmcauley.ucsd.edu/data/amazon/).

---

##  Approach

###  1. Rank-Based Recommendation
- Recommends the **most popular products** based on average ratings and number of interactions.  
- Solves the **Cold Start Problem** by targeting new users.  
- Output: Top 5 products with ≥50/100 interactions.

---

###  2. Similarity-Based Collaborative Filtering
- Finds **similar users** using **Cosine Similarity**.  
- Recommends products that similar users have interacted with but the target user hasn’t.  
- Steps:
  1. Compute user–user similarity scores.  
  2. Retrieve top similar users.  
  3. Recommend new products from those users.

---

###  3. Model-Based Collaborative Filtering (SVD)
- Uses **Singular Value Decomposition (SVD)** on a sparse user–item matrix.  
- Reduces dimensionality to 50 latent features.  
- Predicts ratings and recommends top 5 items per user.  
- Evaluated using **Root Mean Squared Error (RMSE)** between actual and predicted ratings.

---

## Tech Stack
- Python  
- Pandas, NumPy  
- Scikit-learn  
- Scipy (for sparse matrices)  
- Matplotlib / Seaborn (for visualization)

---
