# Unsupervised Learning

The unsupervised part of the project focuses on understanding the intrinsic structure of the data without using target labels.

## Dimensionality reduction

The following methods were used for low-dimensional embedding and visualization:

- **PCA**
- **t-SNE**
- **UMAP**

Both 2D and 3D representations were explored to assess how clearly different cell populations separate in latent space.

A key evaluation metric used in this stage is **trustworthiness**, which measures how well local neighborhood structure is preserved after dimensionality reduction. In some experiments, trustworthiness scores reached values close to **0.96**, indicating that the reduced representation preserved local structure well.

## Clustering methods

The following clustering approaches were explored:

- **K-Means**
- **DBSCAN**

### K-Means
K-Means was typically applied after dimensionality reduction, especially after PCA, in order to group cells into clusters. Performance was analyzed under different configurations, including varying initialization strategies and convergence tolerances.

### DBSCAN
DBSCAN was used to investigate density-based cluster structure and outlier detection. This proved particularly challenging on sparse genomic data, where some parameter settings produced extremely high noise rates, in some cases assigning nearly all points to noise.

## Main takeaway from unsupervised analysis

The unsupervised experiments showed that:

- low-dimensional embeddings, especially **UMAP**, often provide visually meaningful separation between groups
- clustering performance depends heavily on preprocessing choices and data sparsity
- density-based methods can struggle substantially on sparse scRNA-seq datasets