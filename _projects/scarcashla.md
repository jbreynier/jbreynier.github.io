---
title: "sc-arcasHLA: Probabilistic inference of HLA expression variation at the single cell level"
# excerpt: "<br/><img src='/images/scarcashla.png'>"
collection: portfolio
---

![mxTRex overview](/images/scarcashla.png)

HLA dysregulation, either at the DNA or RNA level, plays a crucial role across many cancer types in helping tumors avoid immune detection. However, current analyses focus on bulk sequencing, which is impacted by tumor purity and does not capture within-tumor heterogeneity. I am therefore adapting our tool [arcasHLA](https://github.com/RabadanLab/arcasHLA) for scRNA-seq, allowing for a more precise assessment of HLA expression at the individual cell level.

Analyzing HLA expression in scRNA-seq data presents several difficulties. Poor coverage of HLA alleles, particularly for 3’ sequencing, can result in ambiguous read mapping, since most variable sites are located in exons 2 and 3, away from the 3’ end. Furthermore, data sparsity due to dropouts and high variability in gene expression make it challenging to derive meaningful insights. To overcome these challenges, **I am building a probabilistic model that incorporates ambiguous reads and leverages cell similarity to better estimate the expression distribution of each HLA allele**.
