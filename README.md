# PBMC10k scRNA-seq Analysis (10x Genomics)


## Overview
This project is a short workflow that analyzes the 10x Genomics PBMC10k dataset using Scanpy. The goal of this project is to perform ambient rna removal, doublet detection, QC, normalization, clustering, dimensionality reduction, and manual and automated cell-type annotation.


## Methods
- Dataset: PBMC10k from 10x Genomics (https://www.10xgenomics.com/datasets/10-k-pbm-cs-from-a-healthy-donor-v-3-chemistry-3-standard-3-0-0)
- Workflow: Ambient RNA Removal using soupx → Doublet Detection using SCVI → Normalization → PCA → Clustering using celltypist and leiden → UMAP → Marker  Identification using celltypist and manual research
- Tools: Python, Scanpy, SCVI, SoupX, Leidenalg, CellTypist


## Results
- Identified major immune cell populations (T cells, NK cells, B cells, monocytes, dendritic cells)
- UMAP visualizations included in `/pbmc10k_images`


## How to Run
1. Install dependencies listed in `requirements.txt`
2. Run the notebook `pbmc10k_analysis.ipynb`


## Figures
See `pbmc10k_gallery.md` for UMAPs, QC plots, and Gene Marker dotplots.
