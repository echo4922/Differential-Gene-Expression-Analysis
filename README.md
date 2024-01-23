# Differential-Gene-Expression-Analysis-with-DESeq2

Differential gene expression (DGE) occurs when there is a statistically significant difference or change in read counts or expression levels between two experimental conditions: control and treatment. Therefore, the purpose of differnential expresion analysis is to determine what genes are expressed at different levels between control and treatment. In bulk RNA-Sequencig analysis, the standard "counts" approach of differential gene analysis tool, DESseq2 is one of most popular Bioinformatics tool to perform differential gene expression analyis.

Using a count matrix as input, DESeq2 internally normalizes data with its median ratios. The internal normalization of DESeq2 then adjusts sequencing depth accordingly. The results yield base 2 log fold changes. To deal with low counts in the count matrix, DESeq2 shrinks log fold changes in relation to the count matrix input. Once the internal normalization and shrinkage are performed, Wald Chi-Square test is performed with log fold changes for statistical significance. Benjamini-Hochberg correction is applied to p-values for false discovery rates.

One thing to note is that DESeq2 must be installed via Bioconductor in R. The Bioconductor is a installation manager for biological data focused libraries/packages for R. The attached R notebook file shows step-by-step analysis.

References: https://www.liebertpub.com/doi/10.1089/cmb.2015.0205, https://bioconductor.org/packages/devel/bioc/vignettes/DESeq2/inst/doc/DESeq2.html
