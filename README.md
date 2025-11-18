# CAGNet: A structure-aware clustering-alternated graph network for cell-cell interaction inference in spatial transcriptomics<br>
## Overview:<br>
CAGNet is a novel graph neural network framework that jointly learns node embeddings and cluster assignments in spatial transcriptomics data. The key innovation is an alternating update mechanism that enables continuous interaction between the embedding space and clustering structure:<br>
• Clustering-augmented Representation Learning: Refines node embeddings using both topological information and clustering structures<br>
• Structure-aware Clustering Optimization: Updates cluster centers based on learned representations while preserving spatial relationships<br>
• Bidirectional Optimization: Enables dynamic adaptation of cellular relationships during training<br>
## Quick Start:<br>
### 1.data preprocessing:<br>
Input your raw Spatial Transcriptomics (ST) data into the preprocess.ipynb file to generate processed files for downstream analysis.<br>
**Input Data:**<br>
• filtered_feature_bc_matrix.h5 (Gene expression data)<br>
• tissue_positions.csv (Spatial coordinates data)<br>
**Output Files:**<br>
• gat_embeddings.h5ad (Processed node embeddings)<br>
• gat_adj_sparse_topk.npz (Processed spatial adjacency matrix)<br>
### 2.Training CAGNet:<br>
Input the preprocessed files into the CAGNet.ipynb file for model training and analysis.<br>
**Input Data:**<br>
• gat_embeddings.h5ad<br>
• gat_adj_sparse_topk.npz<br>
**Output Files:**<br>
• Reconstructed cell-cell interaction network<br>
### 3.Results:<br>
For detailed experimental results and comparisons with baseline methods, please refer to our paper.<br>
