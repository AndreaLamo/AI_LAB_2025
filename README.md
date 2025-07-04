# <h1 align="center">*<ins>AI_LAB_2025</ins>*</h1>

## Authors:
- Andrea Lamonarca (andrea.lamonarca@studbocconi.it)
- Antonio Honsell (antonio.honsell@studbocconi.it)
- Fabian Menekshi (fabian.menekshi@studbocconi.it)
- Kevin Shaqiri (kevin.shaqiri@studbocconi.it)

## Project description
In this group project, carried out as part of the course "Mathematical Modelling for Machine Learning", we have critically evaluated and predicted with a ML classifier whether a given epithelial cell sample from the mammary gland is hypoxic or normoxic, using this as an indicator for the presence of breast cancer. In order to achieve this goal, we started by analysing the various datasets for RNA-sequencing data extracted from samples of MCF7 and HCC1806 cells, obtained with SmartSeq and DropSeq sequencing tehcniques. Therefore, we appropriately preprocessed the high-dimensional datasets with dimensionality reduction techniques, implemented suitable unsupervised algorithms for clustering to grasp the degree of separation between hypoxic and normoxic cells (as well as the presence of other clusters and outliers) and finally trained a stacking classifier, based on a logistic regression trained on the output of a variety of models including SVM, KNN and MLP, to derive our predictions and findings.
