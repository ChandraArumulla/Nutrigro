# Nutrigro
Objective: Build a recommendation system for recipes, leveraging collaborative filtering, content-based filtering, and hybrid methods to suggest personalized recipes to users.

Data Loading: Load recipe and user interaction data into pandas DataFrames.

Collaborative Filtering Data Preparation: Prepare interaction data using the surprise library, defining a rating scale and loading data as a Dataset.

Dataset Splitting: Split the user interaction data into training and testing sets for evaluation.

Collaborative Filtering Model Training: Train an SVD model on the training set to learn latent factors for users and recipes.

Model Evaluation for Collaborative Filtering: Test the SVD model on the test set and calculate RMSE to evaluate the model's prediction accuracy.

Text Feature Extraction: Use TfidfVectorizer to transform recipe descriptions into TF-IDF vectors, creating a content-based similarity metric.

Content-Based Model Training: Train a K-Nearest Neighbors (KNN) model on the TF-IDF matrix using cosine similarity to find similar recipes.

Recipe Recommendation with KNN: Define a function to recommend recipes based on content similarity for a specified recipe ID.

Hybrid Recommendation Function: Implement a hybrid recommender that combines collaborative filtering (SVD score) and content-based (KNN score) using a weighted average (alpha).

Hybrid Scoring: Calculate a hybrid recommendation score for a given user and recipe ID, allowing customization of the contribution from each model.

Output Recommendations: Generate recipe recommendations based on either content similarity (KNN) or a hybrid score for user-specific recommendations.

Result Interpretation: Print the RMSE for collaborative filtering, KNN-based recommendations, and hybrid recommendation scores to assess system performance.

Tuning and Improvement: Adjust model parameters, alpha values, or training data as needed to optimize recommendation accuracy and user satisfaction.
