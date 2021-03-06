# Land Explorer for IPA

Explore detailed expression patterns across human tissues directly from IPA’s Isoform Views. Land Explorer for IPA provides interactive plots of gene expression in 51 different human tissues from the GTEx project, for the gene level and individual splice variants. Learn more about the details underlying IPA’s IsoProfiler, and visualize patterns of differential transcript utilization across profiled tissues, or profiled by any metadata.

## Accessing Land Explorer for IPA

IPA users can examine detailed expression patterns across human tissues directly from IPA's Isoform Views.

From IPA's Isoforms View for your gene of interest, click **"View GTEx human tissue expression (Land Explorer)"** to open the web portal, displaying expression information for your gene.

![image_Isoforms2GTEx](../images/Isoforms2GTEx.png)

By default, the RefSeq gene model is used in the **IPA Isoform View** and **Land Explorer for IPA**. If you switch the drop-down box to **Ensembl** in the **IPA Isoform View**, you can view transcript and gene quantification in **Land Explorer for IPA** using the Ensembl gene model.

![image_LandExplorer_SwitchToEnsembl](../images/LandExplorer_SwitchToEnsembl.png)

**Land Explorer for IPA** plots the expression of the splice variants of any human gene in 51 different human tissues. Gene-level expression is also available in Land Explorer (see below).

![image_ipa_in_landexplorer](../images/Ipa_in_landexplorer.png)

You can find detailed information about navigating Land Explorer's [gene and transcript level Views](../Land Views/Gene Level Views/RnaSeqQuantification.md),
and [filtering data](../Using Land Explorer/Filters/Filters.md).

## Tips and Tricks

###	Filtering on metadata

You can use the extensive metadata for each sample in GTEx to focus only on the samples of interest to you, such as Tissue, Gender, etc.

 1.	Find metadata of interest, then select only the categories you want
 * For example, under **Tissue tab**, click **"Check None"** then keep only four tissues.
 2.  Click Apply button to apply the newly created filters

![image_ApplyFilters_IPA_png](../images/ApplyFilters_IPA.png)

### Regrouping on metadata
You can re-organize all samples along the Y-axis based on any metadata. For example, you can find more detailed tissue-level information by grouping on **Tissue Detail Type**. 
 ![image_IPA_regroup_png](../images/IPA_regroup.png)

###	Trellis on metadata
Separate samples out into entirely different charts using the **Trellis** option.

 ![image_IPA_trellis_png](../images/IPA_trellis.png)

### Switch between transcript-level and gene-level View
By default, expression data for your gene of interest is displayed for transcripts, but you can also view gene-level expression information.

 ![image_IPA_switch_Gene_transcript_png](../images/IPA_switch_Gene_transcript.png)

###	Search for a new gene
While you are in **Land Explorer for IPA**, you can search for expression of other genes of interest, simply be typing in your gene's identifier in **Find Gene**.

 ![image_IPA_search_new_gene_png](../images/IPA_search_new_gene.png)

For full access to hundreds of thousands of samples from healthy and disease tissue, please request a trial of the full OmicSoft Land Explorer: https://www.qiagenbioinformatics.com/land-explorer/.
