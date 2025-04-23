# Clustering Analysis on the Forest Cover Dataset 🌲

This project was developed as part of a university course on **Unsupervised Learning**.

## Project Objective
We used a labeled dataset ("Forest CoverType") – but **intentionally ignored the labels** during the analysis.  
The goal was to apply various unsupervised learning techniques, including:
- Clustering (e.g., KMeans, DBSCAN)
- Dimensionality Reduction (e.g., PCA)
- Clustering Quality Metrics (e.g., Silhouette Score)

After clustering, we compared the resulting clusters to the true labels to evaluate how well the algorithms captured meaningful structures in the data.

---

## How to Run
1. Download the original dataset file `covtype.csv` from Kaggle:  
   👉 https://www.kaggle.com/datasets/uciml/forest-cover-type-dataset  
   *(The file is too large to be included in the repository.)*
2. Place the file in the root directory of the project.
3. Run the notebook (`.ipynb`) or script (`.py`) to:
   - Preprocess the data
   - Apply clustering
   - Export results and visualizations

**Note**: The files included in this repo (such as `sampled_data.csv`) are outputs generated from a specific sample used in my analysis.  
If you prefer to work on the full dataset or generate your own sample, feel free to do so.  
There is also a dedicated section in the code that performs normalization on the full dataset – you can run it yourself to reproduce or customize your own version. (#Data loading and normalization)
📌 If you choose to generate your own outputs from the full dataset, it's recommended to give them different file names.  
   This helps avoid confusion or overwriting the sample-based files that are already included in this repository.
---

##  Key Files

- `sampled_data.csv` – A representative sample of 10,000 rows (without labels), constructed to reflect the original data distribution. Useful for faster testing or demonstrations.

- `clustering_performance_results.csv` – A summary table showing the performance of different clustering methods (e.g., KMeans, DBSCAN), including metrics like Silhouette Score and number of clusters.

- `comparison_clusters_pca_vs_normalized.xlsx` – An Excel file containing:
  - The original `Cover_Type` labels
  - Cluster labels produced by KMeans on normalized features
  - Cluster labels after applying PCA followed by KMeans  
  This enables a clear comparison between methods and clustering quality.

---

## 📘 Report Structure
The written report includes:
- Abstract
- Methodology
- Results & Evaluation
- Conclusions
- **Discussion**: An analysis of the gaps between clustering results and true labels, and insights about the clustering quality.

---

