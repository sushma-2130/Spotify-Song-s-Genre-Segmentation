# 🎵 Spotify-Song-s-Genre-Segmentation
Machine learning project for Spotify song clustering and content-based song recommendation.
<div align="center">

### Intelligent Music Clustering & Song Recommendation using K-Means and Cosine Similarity

Discover patterns in Spotify songs by analyzing their audio characteristics, grouping similar songs using K-Means clustering, and recommending similar songs using Cosine Similarity.

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)

![Google Colab](https://img.shields.io/badge/Google%20Colab-Notebook-orange?style=for-the-badge&logo=googlecolab)

![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-black?style=for-the-badge&logo=pandas)

![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-blue?style=for-the-badge&logo=numpy)

![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-yellow?style=for-the-badge&logo=scikitlearn)

![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-blue?style=for-the-badge)

![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-lightblue?style=for-the-badge)

![Gradio](https://img.shields.io/badge/Gradio-User%20Interface-orange?style=for-the-badge)

</div>

---

# 📖 Overview

Music streaming platforms contain a large collection of songs with different musical characteristics. Each song can be described using audio features such as danceability, energy, loudness, acousticness, valence, and tempo.

This project analyzes a Spotify music dataset and uses **Unsupervised Machine Learning** to group songs with similar audio characteristics.

The project uses:

- Data preprocessing
- Exploratory Data Analysis
- Correlation analysis
- Feature scaling
- K-Means clustering
- Elbow Method
- Silhouette Score
- Principal Component Analysis
- Genre and subgenre analysis
- Cosine Similarity
- Song recommendation
- Gradio user interface

The final system allows a user to enter a song name and receive **10 similar song recommendations**.

---

# 🎯 Project Objectives

- Analyze Spotify song characteristics.

- Explore music genres and subgenres.

- Analyze relationships between audio features.

- Group songs based on their audio characteristics.

- Identify meaningful differences between song clusters.

- Visualize song clusters using PCA.

- Build a content-based song recommendation system.

- Provide a simple interactive recommendation interface.

---

# ✨ Features

- 🎵 Spotify Dataset Analysis

- 🧹 Data Cleaning and Preprocessing

- 📊 Exploratory Data Analysis

- 📈 Audio Feature Visualization

- 🔥 Correlation Matrix

- 📏 Feature Standardization

- 🤖 K-Means Clustering

- 📉 Elbow Method

- 📊 Silhouette Score Evaluation

- 🔍 Cluster Analysis

- 🧩 PCA Visualization

- 🎼 Genre and Subgenre Analysis

- 🎧 Cosine Similarity Recommendation

- 🖥️ Gradio Interactive Interface

---

# 📂 Dataset

The project uses a Spotify music dataset containing:

- **32,828 songs**
- **23 original columns**
- **24 columns after adding the cluster column**
- **6 major playlist genres**
- **Multiple playlist subgenres**

### Major Genres

- EDM
- Rap
- Pop
- R&B
- Latin
- Rock

---

# 🎵 Audio Features Used

The clustering and recommendation system uses the following nine audio features:

- Danceability
- Energy
- Loudness
- Speechiness
- Acousticness
- Instrumentalness
- Liveness
- Valence
- Tempo

These features describe important musical characteristics of each song.

---

# 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| Python | Main programming language |
| Google Colab | Development environment |
| Pandas | Data loading and analysis |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Correlation and heatmap visualization |
| Scikit-Learn | Machine learning |
| StandardScaler | Feature standardization |
| K-Means | Song clustering |
| Silhouette Score | Cluster evaluation |
| PCA | Dimensionality reduction and visualization |
| Cosine Similarity | Song recommendation |
| Gradio | Interactive user interface |

---

# 🤖 Machine Learning Techniques

## Data Preprocessing

- Missing Value Checking
- Missing Value Removal
- Duplicate Checking
- Feature Selection
- Feature Standardization

## Exploratory Data Analysis

- Genre Distribution
- Subgenre Distribution
- Descriptive Statistics
- Audio Feature Histograms
- Correlation Matrix

## Clustering

- K-Means Clustering
- Elbow Method
- Silhouette Score

## Dimensionality Reduction

- Principal Component Analysis (PCA)

## Recommendation

- Cosine Similarity
- Top 10 Similar Songs

---

# 🔄 Project Workflow

```text
Spotify Dataset
       │
       ▼
Data Loading
       │
       ▼
Data Understanding
       │
       ▼
Data Cleaning
       │
       ▼
Exploratory Data Analysis
       │
       ▼
Audio Feature Selection
       │
       ▼
Feature Scaling
       │
       ▼
Elbow Method
       │
       ▼
Silhouette Score
       │
       ▼
K-Means Clustering
       │
       ▼
Cluster Analysis
       │
       ▼
PCA Visualization
       │
       ▼
Genre & Subgenre Analysis
       │
       ▼
Cosine Similarity
       │
       ▼
Song Recommendation
       │
       ▼
Gradio Interface
