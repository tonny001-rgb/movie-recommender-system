# Movie Recommendation System (MovieLens 100K)

## Project Overview

This project builds a movie recommendation system using the MovieLens 100K dataset. The system uses collaborative filtering techniques to predict user preferences and recommend relevant movies.

The goal is to simulate real-world recommendation engines used by platforms such as Netflix, YouTube, and Amazon Prime Video.

---

## Business Problem

Modern streaming platforms contain thousands of movies, creating a problem known as **information overload**. Users often struggle to discover content that matches their preferences.

A recommendation system helps solve this by personalizing movie suggestions based on user behavior.

### Why this matters:
- Improves user engagement
- Increases content discoverability
- Enhances user satisfaction and retention

---

## Stakeholders

- Streaming platforms (Netflix-style services)
- Content recommendation systems
- End users seeking personalized movie suggestions

These stakeholders benefit from improved personalization and better content discovery.

---

## Project Objective

The objective of this project is to:

- Learn user preferences from historical ratings
- Predict unknown movie ratings
- Generate Top 5 personalized movie recommendations per user

---

## Dataset

This project uses the MovieLens 100K dataset from GroupLens Research.

### Dataset Overview:
- 100,000+ ratings
- 1,000+ users
- 1,700+ movies

### Key Files:
- u.data → user ratings
- u.item → movie metadata

### Data Limitations:
- Sparse rating matrix (most users rate few movies)
- Cold start problem (new users/movies lack data)
- Ratings may be biased toward popular movies

---

## Methodology

### 1. Data Understanding
- Loaded and explored dataset structure
- Checked for missing values
- Visualized rating distributions and user behavior patterns

### 2. Data Preparation
- Merged ratings and movie datasets
- Structured data for collaborative filtering
- Split data into training and testing sets

### 3. Modeling
- Baseline model using average ratings
- User-based collaborative filtering (KNN)
- Matrix factorization using SVD

Each model was built iteratively to improve prediction accuracy.

---

## Evaluation

Models were evaluated using:

- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)

### Model Comparison:
- Baseline model performed worst
- KNN improved predictions using similarity-based reasoning
- SVD achieved the best performance by learning latent features

### Final Model Selection:
The SVD model was selected as the final model due to its lowest prediction error and ability to capture hidden user-item relationships.

---

## Recommendation System

The final system uses SVD to:

- Predict unseen movie ratings
- Identify user preferences
- Generate Top 5 personalized movie recommendations

---

## Business Impact

This recommendation system improves user experience by reducing search effort and increasing content relevance. For streaming platforms, this leads to:

- Higher user engagement
- Increased watch time
- Better content discovery
- Improved retention rates

---

## Example Output

For a given user, the system returns:

- Movie Title
- Predicted Rating

The top 5 movies are selected based on highest predicted ratings.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Surprise Library (SVD, KNN)
- Matplotlib / Seaborn
- Jupyter Notebook

---

## Repository Structure


