#  Movie Recommendation System (MovieLens 100K)

##  Project Overview

This project builds a **movie recommendation system** using the MovieLens 100K dataset.  
The system recommends movies to users based on their past ratings using **collaborative filtering techniques**.

The goal is to simulate how real-world platforms like Netflix or YouTube recommend content to users.

---

## Business Problem

Users are often overwhelmed by the number of movies available on streaming platforms.  
This creates a problem called **information overload**.

###  Why is this a problem?
- Users struggle to find movies they will enjoy
- Platforms lose engagement if users cannot discover relevant content
- Poor recommendations reduce user satisfaction

###  Stakeholders
- Streaming platforms (Netflix-style services)
- Movie recommendation websites
- Users looking for personalized movie suggestions

---

##  Project Objective

To build a system that:
- Learns user preferences from historical ratings
- Predicts unseen movie ratings
- Recommends the **Top 5 movies** a user is most likely to enjoy

---

##  Dataset

This project uses the **MovieLens 100K dataset** from GroupLens Research.

### Dataset contents:
- 100,000+ ratings
- 1,000+ users
- 1,700+ movies

### Key files:
- `u.data` → user ratings
- `u.item` → movie metadata

---

##  Methodology

The project follows these steps:

### 1. Data Understanding
- Loaded ratings and movie datasets
- Explored data structure
- Visualized rating distribution and user behavior

### 2. Data Preparation
- Merged datasets
- Created user-item matrix
- Split data into training and testing sets

### 3. Modeling
- Built a **baseline model** (average rating predictor)
- Built a **collaborative filtering model (SVD)**
- Compared model performance

### 4. Evaluation
- Evaluated models using:
  - RMSE (Root Mean Squared Error)
  - MAE (Mean Absolute Error)
- Compared baseline vs SVD performance

---

##  Recommendation System

The final model uses **Singular Value Decomposition (SVD)** to:

- Learn hidden patterns in user preferences
- Predict missing ratings
- Recommend the top 5 movies for each user

---

##  Results

- The SVD model outperformed the baseline model
- Lower RMSE and MAE indicate improved accuracy
- The system generates personalized recommendations

---

## Example Output

For a given user, the system returns:

- Movie Title
- Predicted Rating

Top 5 recommended movies are selected based on highest predicted ratings.

---

##  Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Surprise Library (SVD model)
- Matplotlib / Seaborn (visualization)
- Jupyter Notebook

---

##  Repository Structure
├── data/
│ └── ml-100k/
├── movie final notebook.ipynb
├── README.md

