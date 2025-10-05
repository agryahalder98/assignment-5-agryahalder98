# DA5401: A5: Visualizing Data Veracity Challenges in Multi-Label Classification

### **Name:** AGRYA HALDER  

### **Roll:** ED25D900

## 📌 Project Overview

This project addresses the challenges of **data veracity** in **multi-label classification** using the **Yeast dataset**. It focuses on how dimensionality reduction and clustering can reveal the underlying structure of data, which is often a low-dimensional manifold embedded in a high-dimensional space. The key objective is to understand how well these visualization techniques capture the `true` data structure and the implications for classification tasks.


## ⚙️ Methods Implemented

1.  **Dimensionality Reduction**:

      * **Isomap**: Used to reduce the 103 gene expression features down to a 2D space while preserving the geodesic (manifold) distances.
      * **t-SNE**: Employed for non-linear dimensionality reduction, emphasizing the preservation of local neighborhoods in the low-dimensional embedding.

2.  **Clustering Analysis**:

      * **K-Means**: Applied to the dimensionally-reduced data to find natural groupings. The elbow method was used to determine the optimal number of clusters (`k`).
      * **DBSCAN**: Used to identify clusters of varying shapes and density, and to detect outliers.

3.  **Visualization & Evaluation**:

      * Scatter plots of the 2D Isomap and t-SNE embeddings were generated to visually inspect the data's manifold structure.
      * Cluster assignments from K-Means and DBSCAN were overlaid on these plots to assess how well the clusters align with the visual groupings.


## 📊 Evaluation Metrics

  * **Isomap Reconstruction Error**: A quantitative measure of how well the algorithm preserves the original data's distances. A lower value indicates a better job of "unrolling" the manifold.
  * **Qualitative Analysis**: Visual inspection of the plots to infer manifold complexity and the effectiveness of the clustering.

-----

## 🚀 How to Run

1.  Open the Jupyter notebook `DA5401 A5_ED25D900.ipynb` in your environment.
2.  Run all cells to reproduce the analysis, including data loading, dimensionality reduction, clustering, and visualizations.

-----

## File Structure

```
├── DA5401 A5_ED25D900.ipynb   # Jupyter Notebook with full analysis
├── README.md                  # Project documentation
└── yeast.arff                 # The dataset used for this analysis
```
