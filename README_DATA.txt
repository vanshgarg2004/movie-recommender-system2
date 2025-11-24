# Dataset Information for Movie Recommender System

This project uses the **TMDB 5000 Movies Dataset**.

Since GitHub does not allow uploading files larger than 25MB directly, the dataset is not included in this repository.

## 📥 Download Dataset
You can download the dataset from Kaggle using the link below:

🔗 https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata

After downloading, extract the files and place the following CSV files in the project folder:

- tmdb_5000_movies.csv
- tmdb_5000_credits.csv

## ⚙️ Additional Notes
- These CSV files are required for running `movie_recommender.ipynb` and generating the similarity matrix.
- The ready-to-use pickle files (`movies_dict.pkl` and `similarity.pkl`) can be used without downloading the dataset, as long as they are placed in the main project directory.

## ❗ If pickle files are missing
If `movies_dict.pkl` or `similarity.pkl` are not included due to size limits, run the notebook `movie_recommender.ipynb` to regenerate them.

