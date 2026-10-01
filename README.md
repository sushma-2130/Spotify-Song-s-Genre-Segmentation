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

📊 Exploratory Data Analysis

The project performs several exploratory analyses to understand the Spotify dataset.

Genre Analysis

The dataset contains six major genres:

Genre	Number of Songs
EDM	6,043
Rap	5,743
Pop	5,507
R&B	5,431
EDM contains the highest number of songs in the dataset.

Subgenre Analysis

The dataset contains 24 playlist subgenres.

The largest subgenre is:

Progressive electro house — 1,809 songs


🔥 Correlation Analysis

A correlation matrix was created using the nine selected audio features.

Some important observed relationships include:

Energy and Loudness → 0.68
Energy and Acousticness → -0.54
Loudness and Acousticness → -0.36
Danceability and Valence → 0.33

The correlation matrix helps identify relationships between different audio characteristics.
Latin	5,153
Rock	4,951


📏 Feature Standardization

Because the selected audio features have different numerical ranges, StandardScaler was used before clustering.

The scaled feature matrix contains:

32,828 songs
9 audio features

Resulting shape:

(32828, 9)


🤖 K-Means Clustering

K-Means clustering was tested with cluster values ranging from:

K = 2 to K = 10

The Elbow Method was used to analyze inertia.

The Silhouette Score was then calculated to compare the clustering results.

Silhouette Scores
K	Silhouette Score
2	0.1897
3	0.1361
4	0.1494
5	0.1548
6	0.1574
7	0.1407
8	0.1384
9	0.1432
10	0.1418
Among the tested values, K = 2 produced the highest silhouette score of 0.1897


📊 Cluster Results

The final clustering produced two groups:

Cluster	Number of Songs
Cluster 0	9,665
Cluster 1	23,163
Cluster 0 Characteristics

Cluster 0 has:

Lower average energy
Lower average loudness
Higher acousticness
Lower average tempo
Cluster 1 Characteristics

Cluster 1 has:

Higher average energy
Higher average loudness
Lower acousticness
Slightly higher average tempo

Danceability is relatively similar between the two clusters


🔍 PCA Visualization

Principal Component Analysis was used to reduce the nine-dimensional audio feature space to two dimensions for visualization.

PCA Result
PCA Shape: (32828, 2)

Explained variance:

Principal Component 1 = 23.91%
Principal Component 2 = 16.76%

Combined explained variance:

40.67%

The PCA visualization provides a two-dimensional view of the cluster structure.


🎼 Genre Analysis Across Clusters

The distribution of genres across the two clusters was analyzed.

Genre	Cluster 0	Cluster 1
EDM	10.89%	89.11%
Latin	25.46%	74.54%
Pop	25.31%	74.69%
R&B	51.50%	48.50%
Rap	35.33%	64.67%
Rock	29.79%	70.21%

These percentages are calculated within each genre.

The clusters were created using audio features rather than genre labels.


🎧 Subgenre Analysis

The project also analyzed how playlist subgenres are distributed across the clusters.

The largest percentage-point differences were observed for:

Subgenre	Difference
Big room	91.71
Progressive electro house	83.86
Reggaeton	75.32
Hard rock	72.53
Electro house	71.01
Pop EDM	67.96
Dance pop	67.95
Latin hip hop	58.43
Post-teen pop	58.02
Electropop	56.53




EDM contains the highest number of songs in the dataset.

