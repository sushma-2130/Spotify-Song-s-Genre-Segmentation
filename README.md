# 🎵 Spotify-Songs-Genre-Segmentation
Machine learning project for Spotify song clustering and content-based song recommendation.
<div align="center">

### 🎵 Spotify Songs Genre Segmentation using Machine Learning

### Intelligent Music Genre Segmentation & Song Recommendation using K-Means Clustering

Discover hidden patterns in Spotify songs by clustering tracks based on their audio characteristics and generating song recommendations using unsupervised Machine Learning.

[Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python) [Google Colab](https://img.shields.io/badge/Google%20Colab-Notebook-orange?style=for-the-badge&logo=googlecolab) [Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-yellow?style=for-the-badge&logo=scikitlearn) [Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-purple?style=for-the-badge&logo=pandas) [NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-blue?style=for-the-badge&logo=numpy) [Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-green?style=for-the-badge&logo=matplotlib) [Seaborn](https://img.shields.io/badge/Seaborn-Visualization-red?style=for-the-badge) [Gradio](https://img.shields.io/badge/Gradio-Interface-orange?style=for-the-badge) [License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

---

# 📖 Overview

Music streaming platforms contain large collections of songs with different musical characteristics. Understanding similarities between songs can help in music discovery and recommendation systems.

This project applies **K-Means Clustering**, an unsupervised Machine Learning algorithm, to segment Spotify songs based on their audio characteristics. The project analyzes audio features such as danceability, energy, loudness, speechiness, acousticness, instrumentalness, liveness, valence, and tempo.

The project also analyzes how the generated clusters are distributed across **playlist genres and playlist subgenres**.

A **Song Recommendation System** is developed using **Cosine Similarity** to recommend songs with similar audio characteristics. A simple **Gradio interface** is also created to allow users to enter a song name and receive 10 similar song recommendations.

---

# 🎯 Project Objectives

- Analyze Spotify song characteristics.
- Perform data cleaning and preprocessing.
- Explore genre and subgenre distributions.
- Analyze relationships between audio features.
- Discover hidden patterns in Spotify songs.
- Segment songs using K-Means Clustering.
- Determine a suitable number of clusters using the Elbow Method and Silhouette Score.
- Visualize song clusters using PCA.
- Analyze cluster distribution across genres and subgenres.
- Build a song recommendation system using Cosine Similarity.
- Create a simple Gradio interface for song recommendations.
- Demonstrate practical applications of Unsupervised Machine Learning.

---

# ✨ Features

- 🎵 Spotify Dataset Analysis
- 📊 Exploratory Data Analysis (EDA)
- 🧹 Data Cleaning & Preprocessing
- 📈 Genre and Subgenre Analysis
- 📊 Audio Feature Analysis
- 🔗 Correlation Matrix
- 📏 Feature Standardization
- 🤖 K-Means Clustering
- 📈 Elbow Method
- 📊 Silhouette Score
- 🧩 Cluster Analysis
- 📉 PCA Visualization
- 🎧 Song Recommendation System
- 🖥️ Gradio User Interface

---

# 📂 Dataset Features

The Spotify dataset contains song information, playlist information, genre information, and audio characteristics.

### Song Information

- Track ID
- Track Name
- Track Artist
- Track Album ID
- Track Album Name
- Track Album Release Date
- Track Popularity

### Playlist Information

- Playlist Name
- Playlist ID
- Playlist Genre
- Playlist Subgenre

### Audio Features

- Danceability
- Energy
- Loudness
- Speechiness
- Acousticness
- Instrumentalness
- Liveness
- Valence
- Tempo
- Key
- Mode
- Duration

The clustering and recommendation system uses the following **9 audio features**:

- Danceability
- Energy
- Loudness
- Speechiness
- Acousticness
- Instrumentalness
- Liveness
- Valence
- Tempo

After removing missing values, the dataset contained **32,828 songs**.

---

# 🛠️ Technologies Used

| **Technology**   | **Purpose**             |
| ---------------- | ----------------------- |
| Python           | Programming Language    |
| Google Colab     | Development Environment |
| Pandas           | Data Processing         |
| NumPy            | Numerical Computing     |
| Scikit-Learn     | Machine Learning        |
| Matplotlib       | Data Visualization      |
| Seaborn          | Data Visualization      |
| Gradio           | User Interface          |

---

# 🤖 Machine Learning Techniques

### Data Preprocessing

- Missing Value Handling
- Duplicate Checking
- Data Type Analysis
- Feature Selection
- Standard Scaling

### Exploratory Data Analysis

- Genre Distribution
- Subgenre Distribution
- Audio Feature Statistics
- Audio Feature Histograms
- Correlation Matrix

### Clustering Algorithm

- K-Means Clustering

### Cluster Optimization

- Elbow Method
- Silhouette Score

### Dimensionality Reduction

- Principal Component Analysis (PCA)

### Recommendation

- Cosine Similarity based Song Recommendation

---

# 🔄 Project Workflow

```text
Spotify Dataset
        │
        ▼
Data Loading
        │
        ▼
Data Inspection
        │
        ▼
Missing Value Handling
        │
        ▼
Duplicate Checking
        │
        ▼
Exploratory Data Analysis
        │
        ▼
Genre & Subgenre Analysis
        │
        ▼
Audio Feature Analysis
        │
        ▼
Correlation Matrix
        │
        ▼
Feature Selection
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
Genre/Subgenre Cluster Analysis
        │
        ▼
Cosine Similarity
        │
        ▼
Song Recommendation
        │
        ▼
Gradio Interface
📂 Project Structure
Spotify_Genre_Segmentation/

├── Spotify_Genre_Segmentation.ipynb
├── spotify dataset.csv
├── README.md
└── LICENSE
🚀 Installation
Clone Repository
git clone https://github.com/yeswanth096/Spotify_Genre_Segmentation.git
Navigate
cd Spotify_Genre_Segmentation
Install Dependencies
pip install pandas numpy matplotlib seaborn scikit-learn gradio
Launch Notebook

Open the notebook using Google Colab or Jupyter Notebook.

Spotify_Genre_Segmentation.ipynb
📊 Model Pipeline

The implementation follows these stages:

Dataset Loading
Data Exploration
Missing Value Handling
Duplicate Checking
Genre and Subgenre Analysis
Audio Feature Analysis
Correlation Analysis
Feature Selection
Standardization
Elbow Method Analysis
Silhouette Score Evaluation
K-Means Clustering
Cluster Analysis
PCA Visualization
Genre and Subgenre Cluster Analysis
Cosine Similarity
Song Recommendation
Gradio Interface
🎯 Results

The project successfully analyzes and segments Spotify songs based on their audio characteristics.

Dataset
Initial dataset: 32,833 rows
Final dataset after removing missing values: 32,828 rows
Duplicate records after cleaning: 0
Genre Distribution

The dataset contains six major playlist genres:

EDM
Rap
Pop
R&B
Latin
Rock
K-Means Clustering

The Silhouette Scores were evaluated for values of K from 2 to 10.

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

Based on the tested values, K = 2 was selected for the final clustering model.

Final Cluster Distribution
Cluster	Number of Songs
Cluster 0	9,665
Cluster 1	23,163
Cluster Characteristics

Cluster 0 generally contains songs with:

Lower energy
Lower loudness
Higher acousticness
Lower average tempo

Cluster 1 generally contains songs with:

Higher energy
Higher loudness
Lower acousticness
Higher average tempo

The clusters were also analyzed across playlist genres and subgenres to understand how different musical categories are distributed.

PCA Visualization

PCA was used to visualize the song clusters in two dimensions.

The explained variance was:

PC1: 23.91%
PC2: 16.76%
Combined: 40.67%
🎧 Song Recommendation

The recommendation engine uses Cosine Similarity on the nine standardized audio features.

The system takes a song name as input and calculates its similarity with other songs in the dataset.

It then returns the Top 10 most similar songs.

Example

Input Song:

As If It's Your Last
Sample Recommendations
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

The system also provides a similarity score for each recommendation.

🖥️ Gradio Interface

A simple Gradio interface was created for the recommendation system.

Users can enter a song name in the input field, and the system returns a list of 10 recommended songs along with their similarity scores.

Enter Song Name
       │
       ▼
Cosine Similarity
       │
       ▼
Top 10 Similar Songs
       │
       ▼
Similarity Scores
🚀 Future Enhancements
Principal Component Analysis based improved clustering
Hierarchical Clustering
DBSCAN Clustering
Improved clustering evaluation
Interactive Dashboard
Streamlit Web Application
Spotify API Integration
Real-Time Recommendations
Personalized Music Recommendation Engine
Playlist Recommendation System
User Listening History Integration
Advanced Music Embeddings
💡 Applications
Music Recommendation Systems
Song Similarity Analysis
Music Discovery Platforms
Music Streaming Applications
Music Analytics
Audio Content Organization
Genre Discovery
Personalized Music Discovery
Playlist Generation
Unsupervised Music Segmentation
🤝 Contributing

Contributions are welcome.

Feel free to:

Improve clustering performance
Add additional clustering algorithms
Enhance visualizations
Improve the recommendation system
Develop a better user interface
Integrate Spotify API
Optimize the Machine Learning pipeline
Submit pull requests
👨‍💻 Author
Kanna Sushma

Machine Learning & Data Science Enthusiast

GitHub

https://github.com/sushma-2130

📄 License

This project is licensed under the MIT License.

⭐ Support

If you found this project useful, please consider giving it a ⭐ on GitHub.

It motivates future Machine Learning and Data Science projects.

🎵 Discovering Musical Patterns with Unsupervised Machine Learning

Python • Pandas • Scikit-Learn • K-Means • PCA • Cosine Similarity • Spotify Analytics • Gradio

Made with ❤️ by Kanna Sushma
