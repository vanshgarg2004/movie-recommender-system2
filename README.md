# 🎬 Movie Recommender System

🔗 **Live Demo:** https://movie-recommender-system-x77n.onrender.com/

A content-based movie recommendation web app that suggests similar movies based on your selected title.  
Built with **Python, Streamlit, Pandas, scikit-learn**, and the **TMDB 5000 Movies** dataset.

---

## 🚀 Features

- 🔍 Select any movie and instantly get **top 5 similar recommendations**
- 🎭 Uses **content-based filtering** on movie metadata (genres, keywords, overview, etc.)
- 🧮 Precomputed **cosine similarity matrix** for fast recommendations
- 🖥️ Clean and responsive UI built with **Streamlit**
- 🌐 Deployed on **Render** for public access

---

## 🧠 How It Works

1. **Data Loading**  
   Uses `tmdb_5000_movies.csv` and `tmdb_5000_credits.csv` from the TMDB 5000 dataset.

2. **Preprocessing & Feature Engineering**  
   - Merges movies & credits data  
   - Creates a combined `tags` feature using overview, genres, keywords, cast, crew  
   - Converts text to vectors using **CountVectorizer / Bag of Words**

3. **Similarity Computation**  
   - Computes a **cosine similarity matrix** between all movies  
   - Stores processed movie dictionary in `movies_dict.pkl`  
   - Stores similarity matrix in `similarity.pkl` for fast lookup

4. **Streamlit App (`app.py`)**  
   - Dropdown to select a movie  
   - Shows top similar movies with posters  
   - Calls TMDB API (or image URLs from dataset) to fetch posters

---

## 📁 Project Structure

```bash
movie-recommender-system/
├── app.py                     # Streamlit app
├── movie_recommender.ipynb    # Notebook for data cleaning & model building
├── movies_dict.pkl            # Preprocessed movies dictionary
├── similarity.pkl             # Cosine similarity matrix
├── tmdb_5000_movies.csv       # Movies metadata
├── tmdb_5000_credits.csv      # Credits metadata
├── requirements.txt           # Python dependencies
├── screenshot.png             # UI screenshot
└── README.md                  # Project documentation
