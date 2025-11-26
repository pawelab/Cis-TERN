# **Cis-TERN**
**Cis-TERN: a graph-based method to integrate single-cell chromatin accessibility with gene expression data to infer the pseudotime ordering of cells**

[BioRxiv preprint](https://www.biorxiv.org/content/10.1101/2025.11.21.689849v1)

## **Abstract**
Pseudotime ordering methods computationally arrange individually sequenced cells along a continuous trajectory to infer their progression through biological processes. Chromatin accessibility at regulatory elements is pivotal for orchestrating the timing of gene expression during cellular differentiation. However, the sparsity inherent in single-cell data, along with the discrete grouping imposed by clustering-based approaches, often obscures subtle cell-state transitions and intermediate populations. Here, we introduce Cis-TERN (Cis-Temporally Encoded Regulation Network), a graph-based method that integrates single-cell measurements of gene expression (scRNA-seq) and chromatin accessibility (scATAC-seq) to infer a pseudotime ordering of cells. Exploiting the fact that distal cis chromatin accessibility often precedes gene activation, Cis-TERN builds a directed bipartite graph between scRNA-seq and scATAC-seq cells with edge weights determined by either proximal or distal accessibility. Through network diffusion, Cis-TERN assigns continuous pseudotime scores to all cells. Cis-TERN infers cellular pseudotime without the need for prior biological knowledge, such as specifying a root cell type, thereby enabling unbiased reconstruction of differentiation from data alone. We show that our scores align with known lineages in healthy and tumor-derived hematopoietic cells. Additionally, Cis-TERN is able to trace individual cancer cells back to progenitor cell types. Our approach establishes a framework for leveraging chromatin accessibility and gene expression jointly to learn the timing of cell state progression.

## **Demo Notebook**

The notebook **Cis-TERN.ipynb** includes a demo to run Cis-TERN's forward and reverse tracing functionality on the healthy hematopoietic dataset described in the paper.
