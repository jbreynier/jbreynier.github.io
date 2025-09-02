---
title: "mxTRex: Uncovering T-cell transcriptional programs associated with antigen specificity in single cell genomics"
collection: portfolio
---

![mxTRex overview](/images/mxtrex_combined.png)

Single-cell multi-omics enables joint profiling of transcriptomes and T cell receptors (TCRs), and since T cells with similar TCRs often target the same antigens, they tend to share functional states, revealing meaningful cross-modal relationships. However, typical analyses treat gene expression and TCR data separately, with TCRs mapped directly onto expression clusters. I have developped a new method to deconvolute T cell expression signatures guided by TCR information.

My model, mxTRex, performs matrix factorization of the cell by gene expression matrix (G), regularized by a Laplacian cell-by-cell graph of TCR distances (L). The factorization of the expression matrix into gene weights (W) and cell loadings (H) is optimized mainly through two loss functions: a gene expression reconstruction loss, and for a subset of the factors, a TCR graph-regularization loss, guiding those factors to capture expression similarities among T cells with similar TCRs. Thus, **mxTRex reveals gene expression patterns linked to TCR connectivity, identifying antigen-specific expression signatures**.
