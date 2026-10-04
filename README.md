# 🎵 Spotify-Songs-Genre-Segmentation
Machine learning project for Spotify song clustering and content-based song recommendation.
<div align="center">

### # 🎵 Spotify Song's Genre Segmentation using Machine Learning

### Intelligent Music Genre Segmentation & Song Recommendation using K-Means Clustering

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Google Colab](https://img.shields.io/badge/Google%20Colab-Notebook-orange)
![Scikit Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-yellow)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-purple)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-blue)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-green)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-red)
![Gradio](https://img.shields.io/badge/Gradio-UI-orange)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

# 📖 Overview

The **Spotify Song's Genre Segmentation using Machine Learning** project focuses on analyzing Spotify songs based on their audio characteristics and discovering natural groups using **Unsupervised Machine Learning**.

The project uses **K-Means Clustering** to group songs according to their audio features such as:

- Danceability
- Energy
- Loudness
- Speechiness
- Acousticness
- Instrumentalness
- Liveness
- Valence
- Tempo

The project also analyzes how the generated clusters are distributed across **playlist genres and playlist subgenres**.

A **Song Recommendation System** is developed using **Cosine Similarity**, which recommends songs with similar audio characteristics to a selected song.

A simple **Gradio interface** is also created so that users can enter a song name and receive similar song recommendations.

---

# 🎯 Project Objectives

- Perform data preprocessing and cleaning on the Spotify dataset.
- Analyze Spotify songs using statistical methods and visualizations.
- Study the distribution of songs across playlist genres and subgenres.
- Calculate and visualize the correlation between audio features.
- Apply **K-Means Clustering** to segment songs based on audio characteristics.
- Use the **Elbow Method** and **Silhouette Score** to study the suitable number of clusters.
- Visualize clusters using **PCA**.
- Analyze the relationship between clusters and playlist genres and subgenres.
- Build a song recommendation system using **Cosine Similarity**.
- Develop a simple **Gradio user interface** for recommendations.

---

# ✨ Features

### 🎵 Data Preprocessing

- Load Spotify dataset
- Handle missing values
- Check duplicate records
- Analyze data types and dataset structure

### 📊 Exploratory Data Analysis

- Genre distribution analysis
- Subgenre distribution analysis
- Audio feature descriptive statistics
- Audio feature histograms
- Correlation matrix visualization

### 🤖 Song Clustering

- StandardScaler for feature scaling
- K-Means clustering
- Elbow Method
- Silhouette Score
- Cluster summary analysis
- Cluster heatmap
- PCA visualization
- Genre and subgenre cluster analysis

### 🎧 Song Recommendation

- Cosine Similarity based recommendation
- Similarity score calculation
- Top 10 similar songs
- Artist and genre information
- Duplicate recommendation removal

### 🖥️ User Interface

- Gradio based interface
- Simple song name input
- Displays recommended songs and similarity scores

---

# 📂 Dataset Features

The Spotify dataset contains information about songs, artists, playlists, genres and audio characteristics.

### Song Information

- `track_id`
- `track_name`
- `track_artist`
- `track_album_id`
- `track_album_name`
- `track_album_release_date`
- `track_popularity`

### Playlist Information

- `playlist_name`
- `playlist_id`
- `playlist_genre`
- `playlist_subgenre`

### Audio Features

- `danceability`
- `energy`
- `key`
- `loudness`
- `mode`
- `speechiness`
- `acousticness`
- `instrumentalness`
- `liveness`
- `valence`
- `tempo`
- `duration_ms`

After preprocessing, the dataset contained **32,828 songs** and **23 original columns**. One additional `cluster` column was added during clustering, resulting in **24 columns**.

---

# 🛠️ Technologies Used

- **Python**
- **Google Colab**
- **Pandas**
- **NumPy**
- **Scikit-Learn**
- **Matplotlib**
- **Seaborn**
- **Gradio**

---

# 🤖 Machine Learning Techniques

### K-Means Clustering

K-Means is an unsupervised machine learning algorithm used to divide songs into groups based on similarity in their audio features.

In this project, the selected audio features were standardized before applying K-Means clustering.

### Elbow Method

The Elbow Method was used to examine the change in clustering inertia for different values of K.

### Silhouette Score

Silhouette Score was used to compare the quality of clustering for different K values.

The tested scores were:

| K | Silhouette Score |
|---|---:|
| 2 | 0.1897 |
| 3 | 0.1361 |
| 4 | 0.1494 |
| 5 | 0.1548 |
| 6 | 0.1574 |
| 7 | 0.1407 |
| 8 | 0.1384 |
| 9 | 0.1432 |
| 10 | 0.1418 |

Based on the tested values, **K = 2** was used for the final clustering.

### PCA

Principal Component Analysis was used to visualize the song clusters in two dimensions.

The first two principal components explained approximately **40.67%** of the total variance:

- PC1: 23.91%
- PC2: 16.76%

### Cosine Similarity

Cosine Similarity was used in the recommendation system to measure similarity between songs based on their standardized audio features.

---

# 🔄 Project Workflow

Spotify Dataset  
↓  
Data Loading  
↓  
Data Inspection  
↓  
Missing Value Handling  
↓  
Duplicate Checking  
↓  
Exploratory Data Analysis  
↓  
Genre & Subgenre Analysis  
↓  
Audio Feature Analysis  
↓  
Correlation Matrix  
↓  
Feature Selection  
↓  
StandardScaler  
↓  
Elbow Method  
↓  
Silhouette Score  
↓  
K-Means Clustering  
↓  
Cluster Analysis  
↓  
PCA Visualization  
↓  
Genre/Subgenre Cluster Analysis  
↓  
Cosine Similarity  
↓  
Song Recommendation System  
↓  
Gradio Interface

---

# 📂 Project Structure

Spotify_Genre_Segmentation/  
│  
├── Spotify_Genre_Segmentation.ipynb  
├── spotify dataset.csv  
├── README.md  
└── LICENSE

---

# 🚀 Installation

Clone the repository:

    git clone https://github.com/yeswanth096/Spotify_Genre_Segmentation.git

Navigate to the project folder:

    cd Spotify_Genre_Segmentation

Install the required libraries:

    pip install pandas numpy matplotlib seaborn scikit-learn gradio

Open the notebook using **Google Colab** or **Jupyter Notebook**.

---

# 📊 Model Pipeline

### Step 1: Data Cleaning

The dataset initially contained **32,833 rows**.

Five rows contained missing values in:

- `track_name`
- `track_artist`
- `track_album_name`

The missing records were removed.

Final dataset:

- **32,828 rows**
- **23 original columns**
- **24 columns after adding cluster labels**

### Step 2: Feature Selection

The following audio features were selected for clustering and recommendation:

    audio_features = [
        'danceability',
        'energy',
        'loudness',
        'speechiness',
        'acousticness',
        'instrumentalness',
        'liveness',
        'valence',
        'tempo'
    ]

### Step 3: Feature Scaling

    from sklearn.preprocessing import StandardScaler

    scaler = StandardScaler()
    X_scaled = scaler.fit_transform(X)

### Step 4: K-Means Clustering

    from sklearn.cluster import KMeans

    kmeans = KMeans(
        n_clusters=2,
        random_state=42,
        n_init=10
    )

    df['cluster'] = kmeans.fit_predict(X_scaled)

### Step 5: PCA Visualization

PCA was applied to reduce the nine-dimensional audio feature space into two dimensions for visualization.

### Step 6: Recommendation System

Cosine Similarity was applied to compare one selected song against the standardized audio feature vectors of the dataset.

The system returns the **top 10 most similar songs**.

---

# 🎯 Results

The final K-Means model generated **2 clusters**.

| Cluster | Number of Songs |
|---|---:|
| Cluster 0 | 9,665 |
| Cluster 1 | 23,163 |

### Cluster Characteristics

**Cluster 0** generally contains songs with:

- Lower energy
- Lower loudness
- Higher acousticness
- Lower average tempo

**Cluster 1** generally contains songs with:

- Higher energy
- Higher loudness
- Lower acousticness
- Higher average tempo

Danceability values between the two clusters were relatively similar.

### Genre Distribution Across Clusters

| Genre | Cluster 0 | Cluster 1 |
|---|---:|---:|
| EDM | 658 | 5,385 |
| Latin | 1,312 | 3,841 |
| Pop | 1,394 | 4,113 |
| R&B | 2,797 | 2,634 |
| Rap | 2,029 | 3,714 |
| Rock | 1,475 | 3,476 |

The analysis shows that songs from different playlist genres can appear in the same audio-feature cluster because the clustering is based on **audio characteristics rather than genre labels**.

### Subgenre Analysis

The project also compared the generated clusters across the playlist subgenres to understand how different subgenres are distributed within the clusters.

---

# 🎧 Song Recommendation

A song recommendation system was implemented using **Cosine Similarity**.

The system compares the selected song with other songs using the nine standardized audio features and returns the most similar songs.

### Example Input

**As If It's Your Last**

### Sample Recommendations

1. Know No Better (feat. Travis Scott, Camila Cabello & Quavo)
2. Name & Number
3. Suave (Remix)
4. On Replay
5. I Don't Care (with Justin Bieber) - Loud Luxury Remix
6. You and I
7. Fun
8. I Miss You (feat. Julia Michaels) - Cahill Remix
9. Glad You Came
10. joy. (R3HAB Remix)

The recommendation system also displays the **similarity score** for each recommended song.

---

# 🚀 Future Enhancements

- Experiment with additional clustering algorithms such as Hierarchical Clustering and DBSCAN.
- Improve cluster visualization using additional dimensionality reduction techniques.
- Add playlist-based recommendations.
- Build a more advanced recommendation system using multiple similarity techniques.
- Develop a more interactive web application.
- Deploy the recommendation system as an online application.
- Include user preferences and listening history for personalized recommendations.
- Experiment with additional Spotify song attributes for improved recommendations.

---

# 💡 Applications

This project can be applied to:

- Music recommendation systems
- Music discovery platforms
- Song similarity analysis
- Music data analytics
- Playlist generation
- Audio-based song segmentation
- Personalized music discovery

---

# 🤝 Contributing

Contributions are welcome!

You can improve this project by:

- Adding new machine learning techniques
- Improving visualizations
- Enhancing the recommendation system
- Developing a better user interface
- Adding new features to the analysis

To contribute:

Fork the repository  
↓  
Create a new branch  
↓  
Make your changes  
↓  
Commit your changes  
↓  
Create a Pull Request

---

# 👨‍💻 Author

## **Kanna Sushma**

Machine Learning & Data Science Enthusiast

GitHub  
https://github.com/yeswanth096

---

# 📄 License

This project is licensed under the **MIT License**.

---

# ⭐ Support

If you found this project useful, please consider giving the repository a ⭐ on GitHub.

---

## 🎵 Discovering Musical Patterns with Unsupervised Machine Learning

**Python • Pandas • Scikit-Learn • K-Means • PCA • Cosine Similarity • Spotify Analytics • Gradio**

Made with ❤️ by **Kanna Sushma**
