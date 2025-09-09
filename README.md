# 🎵 Music Recommendation with Unsupervised Learning

This project explores **unsupervised learning techniques** to discover hidden patterns in music listening behavior.  
Using the [LastFM 1K dataset](http://ocelma.net/MusicRecommendationDataset/lastfm-1K.html), which contains the listening history of ~1,000 users, we build data representations and apply dimensionality reduction, clustering, and latent factor models to understand user preferences and artist/song relationships.

The goal is to uncover **similarities between users, artists, and songs** without labels, and to experiment with **projection methods and recommendation approaches**.

---

## 📑 Contents

### 1. Data Preparation (LastFM 1K)
- Load and clean the dataset  
- Remove duplicate user–artist–song entries  
- Filter out songs with very low popularity  
- Build unique user, artist, and song indices + mapping dictionaries  

### 2. Co-occurrence Matrices
- Construct **user–artist** and **user–song** matrices  
- Represent as **sparse matrices** (`csr_matrix`) for efficiency  
- Calculate sparsity levels  

### 3. Dimensionality Reduction & Visualization
- Project high-dimensional user vectors to 2D  
- Compare **PCA, t-SNE, and UMAP**  
- Justify selection of **UMAP** for scalability and handling of new users  

### 4. Topic Modeling with LDA (Latent Dirichlet Allocation)
- Model latent "topics" of music preferences  
- Group users by probabilistic affinity to artist/song clusters  

### 5. Matrix Factorization with ALS (Alternating Least Squares)
- Decompose user–song interactions  
- Learn latent factors for recommendations  
- Build a recommendation engine  

### 6. Optional: Item2Vec (Word2Vec-style Embeddings)
- Explore algebraic projections of items (songs/artists)  
- Compare embeddings to factorization models  

### 7. Analysis & Results
- Visualize clusters of users with similar listening patterns  
- Interpret latent dimensions from LDA and ALS  
- Generate personalized music recommendations  

---

## 🚀 Key Takeaways
- Built efficient **user–content interaction matrices** from raw listening data.  
- Applied **unsupervised learning methods** (UMAP, LDA, ALS) to extract hidden structure.  
- Demonstrated a **music recommendation pipeline** without explicit labels.  

