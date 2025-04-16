# EpilepsyGenes
## Introduction
In this study, we investigated relationships between genes associated with epilepsy using PubMed. First we used the pubmed.mineR package in R to search for abstracts that were dated from 8th December 2023 and 8th December 2024, and contained both of the terms 'Epilepsy' and 'Gene'. From this, we found 1373 abstracts that met the criteria. We then used latent semantic analysis, where we constructed a matrix showing the frequency of each gene in each abstract. Using this matrix, we found the relationships between each gene. For example, two genes that appear often in the same abstracts will have a higher level of association compared to two genes that never appear in the same abstract. The igraph package was then used to visualize the relationships between the genes. 

Since clusters may exist in the data, where a family of genes are highly associated with each other, and not associated with any gene outside of the family, we used the walktrap algorithm to identify these clusters. The largest eight clusters that were identified using the walktrap algorithm have been coloured. The igraph diagram was then imported into Gephi to make the graph interactive.   

## Diagram

![Epilepsy_Genes_new](https://github.com/user-attachments/assets/e7500f99-808d-4a78-82d7-cc0e330c7fa4)

Click this link for an interactive version of the diagram:
https://albert-l-phan.github.io/EpilepsyGenes/
