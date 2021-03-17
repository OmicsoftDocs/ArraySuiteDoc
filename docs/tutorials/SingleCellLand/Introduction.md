# Introduction
## Single Cell Lands

OmicSoft's new Single Cell Land framework extends the revolutionary OmicLand Framework (OncoLand and DiseaseLand) to deliver large results from curated scRNA-seq projects. 
Single Cell Lands extend the DiseaseLand and OncoLand results, enabling exploration of normal expression, as well as oncology and disease-focused data. 
Land files are built up based on OmicSoft File System (OFS), which stores genomics data in database files and different layers of indexes for gene/markers and samples/cell clusters.

This tutorial will introduce the key visualizations of Single Cell Lands, designed to accelerate discovery of relevant curated datasets and expression for your work.

## Curation and processing
OmicSoft's teams of biologists and bioinformaticians manually process and curate every project in Single Cell Lands to maximize the ability to discover, explor, and cross-compare data.

* Project metadata evaluation
** Is the project compatible with the platform?
** Are all necessary metadata available from the data submission?
** Are results interpretable in context of the paper?
* Data retrieval
** Are data available?
*** Preferred: Raw FASTQ files or BAM
*** Special Lands: processed quantification matrices
** Is the data submission complete, with necessary parsing/processing information?
* Metadata curation
** Extract/curate project, technical, sample, and clinical metadata
** Apply controlled vocabularies and curation standards
** Curate expected results from paper, such as clustering experiments, cell types, and key markers/differentially expressed genes
* Data Processing
** Alignment, quantification, normalization, and post-processing QC
** Dimension reduction/clustering to reproduce paper's key findings
** Statistical comparisons between clusters
* Manual Cell type Annotation
** Manual curation of predicted clusters
*** Overlay key marker genes
*** Confirm proper cluster isolation of expected cell types

The output of this extensive curation process, including project, sample, and curated cell cluster metadata, cell-level gene expression results, and differential expression, are all accessible through the Land interface.
## Land Organization
To enable discovery of relevant datasets that you might not be looking for, diverse projects are gathered in Single Cell Lands, separated by species (human or mouse) and technology (UMI or nonUMI).
### Non-UMI Datasets
Full transcript (non-UMI) scRNAseq datasets such as SMART-seq will be found in Lands such as "SingleCellHuman". Typically fewer cells are measured per experiment, but less gene dropout.
### UMI Datasets
3' and 5' Tag-based technologies enable highly parallel measurement of single cell expression, but does not detect full transcripts, instead only labeling the 5' or 3' end of the transcript.
### Special datasets
Some Lands, such as SingleCellHCL, were processed directly from expression matrices and fully curated, so will be on a different gene model from other Lands.

## Distribution Views
Click **Select Land** and choose SingleCellHuman_B37.

When you open a Single Cell Land, you will first see a "distribution view", indicating the number of datasets available at a level of organization, such as Project, Sample, Cluster, and Comparison.
Use these Views to get a high-level understanding of available data.

In SingleCellHuman, the default distribution View is Cluster Distribution.

### Cluster Distribution

![NewImage1_png](images/201510-01.png)

### Sample Distribution

The **Samples** view shows the number of biological samples in each dataset. 
In the Task tab (right side) use "Specify Histogram columns" to regroup data by Tissue, Disease, or other sample-level metadata, or aggregate by Project metadata. 
Use "Specify Group column" to split each bar further by metadata.
 

![NewImage2_png](images/201510-02.png)

One useful view is **Clinical Significance - Group Association**. It is a dynamic view showing the association of all clinical variables with the selected grouping (sample variable).

![NewImage3_png](images/201510-03.png)

**Survival Data** view is a plot of percent survival across time (Kaplan-Meier Survival Curve) using a specific grouping (e.g. Tumor Type)

![NewImage4_png](images/201510-04.png)

## CCLELand

The Cancer Cell Line Encylopedia (CCLE) project is an effort to conduct a detailed genetic and pharmacologic characterization of a large panel of human cancer cell lines. The CCLE provides public access to genomic data, analysis and visualization of DNA copy number, mRNA expression, mutation data and more, for about 1000 cell lines.

![NewImage5_png](images/201510-04.png)
