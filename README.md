# <h1 align="center">*<ins>AI_LAB_2025</ins>*</h1>

## Authors:
- Andrea Lamonarca (andrea.lamonarca@studbocconi.it)
- Antonio Honsell (antonio.honsell@studbocconi.it)
- Fabian Menekshi (fabian.menekshi@studbocconi.it)
- Kevin Shaqiri (kevin.shaqiri@studbocconi.it)

## Project description
In this group project, carried out as part of the course "Mathematical Modelling for Machine Learning", we have critically evaluated and predicted with a ML classifier whether a given epithelial cell sample from the mammary gland is hypoxic or normoxic, using this as an indicator for the presence of breast cancer. In order to achieve this goal, we started by analysing the various datasets for RNA-sequencing data extracted from samples of MCF7 and HCC1806 cells, obtained with SmartSeq and DropSeq sequencing tehcniques. Therefore, we appropriately preprocessed the high-dimensional datasets with dimensionality reduction techniques, implemented suitable unsupervised algorithms for clustering to grasp the degree of separation between hypoxic and normoxic cells (as well as the presence of other clusters and outliers) and finally trained a stacking classifier, based on a logistic regression trained on the output of a variety of models including SVM, KNN and MLP, to derive our predictions and findings.

## Repo Structure:
```text
.
├─ README.md
├─ LICENSE
├─ .gitignore
├─ requirements.txt          
├─ notebooks/
│  ├─ 01_eda_preprocessing/
│  │  ├─ README.md
│  │  ├─ eda_dropseq.ipynb
│  │  ├─ eda_smartseq_filtered_normalized.ipynb
│  │  ├─ eda_smartseq_unfiltered.ipynb
│  │  └─ isolation_forest_dropseq.ipynb
│  ├─ 02_unsupervised_analysis/
│  │  ├─ README.md
│  │  ├─ dimred_hcc_dropseq.ipynb
│  │  ├─ dimred_hcc_smartseq.ipynb
│  │  ├─ dimred_mcf7_dropseq.ipynb
│  │  ├─ dimred_mcf7_smartseq.ipynb
│  │  ├─ unsupervised_dropseq.ipynb
│  │  └─ unsupervised_smartseq.ipynb
└─ ├─ 03_supervised_analysis/
   │  ├─ README.md
   │  ├─ supervised_hcc_dropseq_smartseq.ipynb
   │  └─ supervised_mcf7_dropseq_smartseq.ipynb
   └─ 04_additional_experiments/
      └─ README.md
   ```

## Key Results
Some of the main conclusions of the project are:

- **Feature selection mattered significantly**, as retaining informative genes was crucial for strong predictive performance.
- **UMAP provided strong visual separation** of groups in reduced space.
- **DBSCAN was highly sensitive to sparsity**, sometimes labeling most observations as noise.
- the comparison between **SmartSeq** and **DropSeq** highlighted meaningful trade-offs between sensitivity, throughput, and downstream modeling behavior.
- **Supervised models performed well**, especially when trained on appropriately filtered datasets.
