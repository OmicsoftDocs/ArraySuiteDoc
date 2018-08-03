# Integration views

Omicsoft Lands have a number of OmicData types (such as copy number variation, expression and mutation data). In addition to viewing individual data types for samples, users can easily integrate these data types in integration views in Land Explorer. For example, users may be interested in whether a gene's copy number status correlates with its expression status. Alternatively, one may be interested in how well microarray and RNA-seq expression values of a gene correlate (where available).


## Microarray Expression vs. RNA-seq Expression

![LandPortal_login_png](../../images/ExpressionRationFPKM_Views.png)

This view shows a single chart, for each gene, comparing Gene Expression Ratio (Sample vs Universal Human Reference) vs Gene Expression (Log2(RPKM + 0.1)). A value of 0.1 has been added to every RPKM value in order to log the data and account for potential values of 0.

## Copy Number Variation (CNV) vs. RNA-seq Expression

![CNVvsFPKM_png](../../images/CNVvsFPKM.png)

This view shows a single chart, for each gene, comparing Gene Expression Ratio (Sample vs Universal Human Reference) vs Average Copy Number Log2 Ratio. By default, all sample types (tumor and normal) are shown, users could visualize a geneset (multiple genes), and choose grouping by Tumor Type, Sample ID, Sample Type, Disease, etc.

## Copy Number Variation (CNV) vs Microarray Expression

Similar to the CNV vs RNA-Seq Expression view, when CNV and Microarray data is available for a gene, pairwise comparison of the two data points (y- and x-axis, respectively) can be done to see if there is a correlation between copy number and expression:

![CNVvsMicroarray](../../images/cnv_microarray.png)



## CNV Expression Ratio

CNV Expression Ratio view shows a single chart, for each gene, comparing Gene Expression (e.g. Sample vs Universal Human Reference) vs Average Copy Number Log2Ratio.

![CNV_expression_ratio_png](../../images/CNV_expression_ratio.png)


## CNV RNA-Seq Expression

CNV RNA-Seq expression view shows a single chart, for each gene, comparing Gene Expression (RPKM) vs Average Copy Number Log2 Ratio.

![CNV_RNA_Seq_Expression_png](../../images/CNV_RNASeq_Expression.png)
