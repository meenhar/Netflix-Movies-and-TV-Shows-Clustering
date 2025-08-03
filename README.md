# 🎬 Netflix Movies & TV Shows Clustering

This project uses **unsupervised machine learning** to cluster Netflix content (movies and TV shows) based on attributes like genre, rating, duration, and textual description. The goal is to group similar titles to improve recommendations and content insights.

---

## 📁 Dataset Overview

- **Source**: Netflix Titles Dataset (CSV)
- **Total Records**: 7,787
- **Key Features**:
  - Type (Movie/TV Show)
  - Genre (listed_in)
  - Rating
  - Duration
  - Description
  - Release Year

---

## 🛠️ Tools and Technologies

- Python (Pandas, NumPy)
- Scikit-learn (TF-IDF, KMeans, DBSCAN, Hierarchical)
- Matplotlib, Seaborn (Visualization)
- Jupyter Notebook

---

## 🔧 Key Steps

1. **Data Preprocessing**  
   - Handled missing values  
   - Converted duration to minutes  
   - Encoded categorical columns  

2. **Feature Engineering**  
   - Extracted main genre  
   - Calculated content age  
   - One-hot encoded genre & type  

3. **Text Vectorization**  
   - Applied **TF-IDF** on the description column  
   - Selected top 100 TF-IDF features  

4. **Clustering Models Used**  
   - K-Means (best performance)  
   - Hierarchical Clustering  
   - DBSCAN (noise-based clustering)

---

## 📊 Model Evaluation

| Model         | Silhouette Score | Notes                        |
|---------------|------------------|------------------------------|
| K-Means (k=4) | ~0.48            | Best separation of clusters  |
| Hierarchical  | ~0.42            | Interpretable structure      |
| DBSCAN        | Varies           | Fewer clusters, sparse data  |

---

## 🔍 Cluster Insights

- **Cluster 0**: Kids and short-duration content  
- **Cluster 1**: Long-form dramas and series  
- **Cluster 2**: Documentaries and international content  
- **Cluster 3**: Mixed content with moderate duration  

---

## ✅ Conclusion

- Successfully grouped Netflix titles using content and description features.
- Clusters reveal strong patterns in **genre**, **duration**, and **audience**.
- Can assist in:
  - Content recommendation systems  
  - Genre-based content organization  
  - Targeted marketing

---



---

