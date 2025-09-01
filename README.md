# Clustering-On-Wine-Dataset
This project applies **unsupervised learning techniques** to the **Wine dataset** from `sklearn.datasets`.  
The aim is to explore and analyze the natural grouping of data points using clustering algorithms.  

---

## Analysis  
- The **Wine dataset** contains 178 samples of wines with 13 chemical features each.  
- The target labels represent the actual wine cultivator classes (not used in training for unsupervised learning).  
- Three clustering algorithms are implemented:  
  1. **K-Means Clustering**  
  2. **Hierarchical Clustering (Agglomerative)**  
  3. **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)**  

---

## Summary  
The project demonstrates:  
1. Loading and exploring the Wine dataset.  
2. Applying different clustering techniques.  
3. Visualizing clusters using **PCA (Principal Component Analysis)** to reduce data to 2D.  
4. Comparing results against actual labels to evaluate clustering performance.  

---

## Results  
- **K-Means Clustering**: Groups the wines into clusters based on Euclidean distance. Works well but requires pre-defining the number of clusters.  
- **Hierarchical Clustering**: Provides a dendrogram to visualize the merging process. Helps understand hierarchical relationships between clusters.  
- **DBSCAN**: Identifies clusters based on density and marks outliers as noise. Effective when clusters are irregularly shaped.  

---

## Analysis and Insights  
- K-Means achieved reasonable separation but was sensitive to the choice of `k`.  
- Hierarchical clustering revealed cluster hierarchies and relationships but sometimes merged clusters prematurely.  
- DBSCAN successfully detected noise points but required careful tuning of `eps` and `min_samples`.  
- PCA visualization showed clear separation between some wine classes, validating the clustering results.  

---

## Recommendations  
- Try **silhouette score** or **Davies–Bouldin index** for more objective evaluation of cluster quality.  
- Experiment with **Gaussian Mixture Models (GMMs)** for probabilistic clustering.  
- Scale features before clustering to avoid bias from larger-valued features.  
- Apply clustering to larger, real-world datasets to test scalability.
