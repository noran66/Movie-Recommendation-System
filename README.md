# 🎬 Movie Recommendation System – Elevvo Internship

For the fifth internship task, I worked on building a **Movie Recommendation System** using the **MovieLens 100K Dataset**.  
The goal was to recommend movies to users based on their past ratings using two main approaches:  

1. **Item-Based Collaborative Filtering**  
2. **Matrix Factorization (SVD)**  

---

## ✅ Steps
- Loaded the **MovieLens 100K dataset** (`u.data`).  
- Preprocessed data by creating a **User-Item Rating Matrix**.  
- Split the dataset into **train** and **test** sets.  
- **Item-Based Collaborative Filtering**:  
  - Calculated cosine similarity between movies.  
  - Recommended movies based on items similar to those rated by the user.  
- **Matrix Factorization (SVD)**:  
  - Applied `TruncatedSVD` to decompose the user-item matrix.  
  - Predicted ratings for unseen movies.  
  - Recommended top-rated unseen movies.  
- **Evaluation**:  
  - Used **Precision@K** to measure recommendation quality.  

---

## 📊 Results (for User ID = 10)
- **Item-Based Recommendations:**  
  `[174, 204, 191, 423, 172, 173, 210, 182, 211, 79]`  

- **SVD Recommendations:**  
  `[483, 182, 514, 523, 12, 143, 582, 508, 432, 204]`  

- **Precision@5**:  
  - Item-Based CF → **0.4**  
  - SVD → **0.6**  

---

## 🔎 Insights
- **SVD outperformed Item-Based CF**, achieving higher precision.  
- Matrix Factorization captures hidden patterns in user preferences more effectively than similarity-based methods.  
- Item-based CF still provides reasonable recommendations, especially when interpretability is important.  

---

## ✅ Conclusion
- Recommendation systems can be built using different approaches.  
- **Matrix Factorization (SVD)** tends to generalize better and provide more accurate predictions.  
- Such systems are crucial for platforms like Netflix, Amazon, and Spotify to personalize user experiences.  

---

📂 **Full code + analysis is available on GitHub:**  
👉 [Movie Recommendation System Repo](https://github.com/noran66/Movie-Recommendation-System.git)
