# Comparison views

The OmicSoft Land curation teams carefully curate samples in the Land using a controlled vocabulary for each project. For each project containing RNA-seq or microarray data, the curation team will generate sample groupings (often matching the ones used by the authors, as well as other meaningful ones) such as Disease vs Normal samples, or Treatment vs. Control samples. The Land Explorer allows users to browse gene level information for these types of comparisons in a simple "bubble plot" view. When searching a gene, and choosing this view, the fold change of the gene will be plotted (each bubble, or dot represents a single comparison). The y-axis will group the comparisons by the primary grouping category, while the x-axis will represent the Log2 Fold change of that gene. The size of the dots will reflect the p value from the comparison (DESeq2 for RNA-seq and General Linear Model for microarray). Selecting dot(s) in this view will populate a Details table at the bottom of the view showing some key metadata from the comparison(s)

The views below can be filtered to comparisons of interest. For information on customizing comparison views, please see: [Comparison Filter](../../Using Land Explorer/Comparison_filters.md)

## All Comparisons

This view combines all comparisons for a gene into one view. In this view, all of the different types of comparisons in the select Land will be plotted:

 ![LandPortal_login_png](../../images/AllComparison.png)

## Disease vs Normal

This view shows all comparisons where samples from affected subjects (i.e. Tumors or Disease) are compared to samples from normal subjects in the same project:

 ![Disease_vs_Normal_png](../../images/DiseasevsNormal.png)

## Treatment vs Control

This view shows all comparisons where samples from affected subjects (treated with drug or other therapy) are compared to samples from untreated subjects in the same project:

 ![Treatment_Vs_control_png](../../images/treatmentvscontrol.png)

## Responder vs NonResponder

This view shows all comparisons where samples from subjects that show favorable response to a treatment are compared to samples from subjects with no response to the same treatment in the same project:

 ![responder_vs_nonresponder_png](../../images/respondervsnonresponder.png)

## Resistant vs Sensitive

This view shows all comparisons where samples from subjects that show resistance to a treatment are compared to samples from subjects showing significant difference in outcome to the same treatment in the same project:

![resistant_vs_sensitive_png](../../images/resistantvssensitive.png)

## Cell Type1 vs Cell Type2

This view shows all comparisons where samples of one cell type from a subject are compared to samples another cell type from these subjects in the same project:

 ![Celltype1_vs_Celltype2_png](../../images/celltype1vscelltype2.png)

## Disease1 vs Disease2


This view shows all comparisons where samples from subjects presenting one disease are compared to samples from other subjects presenting another disease in the same project:

 ![Desease1_vs_deasease2_png](../../images/desease1vsdisease2.png)

## Treatment1 vs Treatment2

This view shows all comparisons where samples from subjects undergoing one treatment are compared to samples from other subjects undergoing a different treatment in the same project:

 ![Treatment1_vs_treatment2_png](../../images/treatment1vstreatment2.png)

## Tissue1 vs Tissue2

This view shows all comparisons where samples of one tissue from a subject are compared to samples another tissue from these subjects in the same project:

 ![Tissue1_vs_tissue2_png](../../images/tissue1vstissue2.png)

## OtherComparisons

This view shows all comparisons that do not fall under the standard categories above:

 ![Other_comparisons_png](../../images/othercomparisons.png)
