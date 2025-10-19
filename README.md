# Book-Recommendation-Engine-KNN
A machine learning project using K-Nearest Neighbors to recommend similar books based on user ratings. Built in Google Colab using the Book-Crossings dataset, applying data cleaning, filtering, and similarity modeling to suggest books with similar reader profiles.
# 📚 Book Recommendation Engine using KNN

This project builds a **Book Recommendation System** using the **K-Nearest Neighbors (KNN)** algorithm. It recommends books that are similar to a given book based on user ratings from the **Book-Crossings dataset**.

---

## 🚀 Features
- Uses **Book-Crossings dataset** (270,000+ books, 1.1M ratings)
- Filters data to ensure statistical significance
- Builds a similarity model using `NearestNeighbors` from `sklearn`
- Returns 5 most similar books for a given title
- Built and tested on **Google Colab**

---

## 🧩 Tech Stack
- Python
- Pandas
- NumPy
- scikit-learn
- Google Colab

---

## 📘 How It Works
1. Clean and filter dataset:
   - Remove users with <200 ratings
   - Remove books with <100 ratings
2. Create a pivot table of ratings
3. Use `NearestNeighbors` to compute book similarities
4. Define function `get_recommends(book_title)` to return:
   ```python
   [
     'Book Title',
     [
       ['Similar Book 1', distance1],
       ['Similar Book 2', distance2],
       ...
     ]
   ]
