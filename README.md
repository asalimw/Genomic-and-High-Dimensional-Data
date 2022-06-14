# Genomic-and-High-Dimensional-Data

###### Visualization and Clustering tools 

We will analyze a single-cell RNA-seq dataset compiled by the Allen Institute with the goal of unveiling hierarchical structure and discovering important genes. The data set contains cells from a mouse neocortex (region in the brain which governs perception and cognition). The datesets provided are all different subsets of a larger single-cell RNA-sqe dataset.

The single-cell RNA-seq data comes in the form of a counts matrix where
- Each row corresponds to a cell. 
- Each column corresponds to the normalized transcript compatibility count (TCC) of an equivalance class of short RNA sequences, rescaled to units of counts per million.
- The TCC entry (i, j) of the data matrix as the level of expression of gene j in cell i.  

Download [Gene Analysis Data - tar.gz file ](https://courses.edx.org/assets/courseware/v1/1affe599859bb7f0ab6facbef4a091ce/asset-v1:MITx+6.419x+3T2021+type@asset+block/release_gene_analysis_data.tar.gz) in three folders:

1. p1, which is a small, labeled subset of the data. It contains the count matrix  along with “ground truth" clustering labels , which were obtained by scientists using domain knowledge and statistical testing.
2. p2_unsupervised, which contains only a count matrix. 
3. p2_evaluation, which contains a labeled training and test set.

The p2_unsupervised_reduced and p2_evaluation_reduced folders contain datasets with a reduced number of genes, in case you are unable to run some of the procedures on the larger versions. In particular, a full logistic regression could take 1 or 2 GB of memory to run.

The data consists of a counts matrix in file Y and X , along with ground truth labels . The ground truth labels are not necessary for this part, but you may use them to verify that your results are sensible.  Goal: Unveil hierarchical structure of the genes and discover important genes.
