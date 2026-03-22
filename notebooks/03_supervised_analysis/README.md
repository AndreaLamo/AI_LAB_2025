# Supervised Learning

The supervised part of the project evaluates how accurately machine learning models can classify cell categories or conditions based on gene expression data.

## Models explored

Several classification models were implemented and compared, including:

- **Random Forest (RF)**
- **Multi-Layer Perceptron (MLP)**
- **Support Vector Machine (SVM)**
- **K-Nearest Neighbors (KNN)**
- **XGBoost (XGB)**

At the end, ensemble and stacking-style approaches were also considered to combine the predictive strengths of multiple models.

## Main takeaway from supervised analysis

The supervised models achieved strong performance, particularly on filtered **DropSeq** datasets. The results suggest that careful preprocessing and preservation of biologically informative gene subsets are essential for maintaining classification quality.