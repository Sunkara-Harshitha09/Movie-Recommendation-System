# Movie-Recommendation-System
Movie Clustering Based on User Reviews
**Project Overview**

This project performs clustering on movies based on user review patterns using unsupervised machine learning techniques. The goal is to group movies that have similar audience response patterns using features derived from rating data.

The project uses the MovieLens ratings dataset and applies clustering algorithms to identify patterns in movie popularity and rating quality.

**Problem Statement**

The objective of this project is to cluster movies based on user reviews. Since the dataset does not contain predefined labels, unsupervised learning techniques are used to automatically group movies with similar characteristics.

Movies are clustered based on:

Average rating

Number of reviews

**Dataset**

Dataset used: MovieLens Ratings Dataset

File used:

ratings_small.csv

Dataset columns:

userId – ID of the user who rated the movie

movieId – Unique movie identifier

rating – Rating given by the user (scale 1–5)

timestamp – Time when the rating was given

Dataset used: MovieLens Ratings Dataset

https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset

File used:
ratings_small.csv
ratings.csv

**Feature Engineering**

The dataset contains user-level ratings, so the data is aggregated to obtain movie-level features.

Features used for clustering:

Average Rating – Mean rating received by a movie

Number of Reviews – Total number of ratings received by a movie


**Data Preprocessing**

The following preprocessing steps were applied:

Data loading and cleaning

Aggregating ratings to movie-level features

Feature scaling using StandardScaler

Creating feature matrix for clustering

Feature matrix used:

avg_rating

num_reviews

**Machine Learning Models**

Two clustering algorithms were applied:

KMeans Clustering

KMeans groups movies based on similarity between features by minimizing the distance between points within a cluster.

Hierarchical Clustering

Agglomerative hierarchical clustering builds clusters step by step by merging similar data points.

**Visualization
**
To understand clustering results, several visualizations were created:

Scatter plot of average rating vs number of reviews

Cluster visualization using KMeans

PCA visualization to reduce dimensions and observe clusters

These visualizations help identify patterns in movie popularity and rating behavior.


**Results**

The clustering results reveal that movies naturally form groups based on audience feedback.

Example cluster patterns:

High rating + high number of reviews → Popular blockbuster movies

High rating + low number of reviews → Underrated movies

Medium rating + medium popularity → Average movies

Low rating + low popularity → Less popular movies

**Conclusion**

This project demonstrates how unsupervised learning techniques can identify patterns in movie review data and group similar movies together.

Clustering helps in understanding audience behavior and can be useful for:

Movie recommendation systems

Content categorization

Audience preference analysis


**Technologies Used**

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

Google Colab
