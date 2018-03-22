# Summary Gene FPKM

## Summary Gene FPKM, RNASeq Transcript View in Land Portal

![LandPortal_login_png](../../images/SummaryGeneFPKM.png)

### Introduction
For each gene, this view shows % of tumor samples whose RNA-Seq expression is 2x up-regulated or 2x down-regulated, compared to normal samples in each group (e.g. Tumor Type). Group is specified by Grouping, and is PrimaryGrouping by default.

### Values
For each group, expression for normal samples is calculated as the average of Log2(FPKM + 0.1). For each tumor sample if its Log2(FPKM + 0.1) is larger than normal sample average by ExpressionUpRegulationCutoff or is smaller than normal average by ExpressionDownRegulationCutoff, this tumor sample is counted as up-regulated or down-regulated.

The percentage showing on Y axis = ( # of tumor samples up-regulated or down-regulated) / ( # of all tumor samples in this group).

### Filters
Fold change cutoff can be changed under Expression in the left panel.
