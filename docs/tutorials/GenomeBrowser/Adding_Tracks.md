# Adding Tracks

A number of data types can be added as tracks including:

*   Alignment files, e.g. BAM, SAM
*   Files with standard format, e.g. BED, bedGraph, GTF, VCF, BigWig
*   Tab-delimited text files containing genomic coordinate information columns (chromosome, start, end)
*   Pre-built mapping tracks by Omicsoft, e.g. Affymetrix probes and probesets track, SNP
*   Data sets in Analysis tab of Array Studio, e.g. NGS data sets, variable view of -omic data sets

This section focuses on adding next generation sequencing data files (BAM files). A common task is to add alignment tracks, e.g. BAM files. The BAM alignment track can display a variety of information such as coverage, exon junctions, pileup, profiles, sequences, and variations.

In this tutorial we will add BAM files from a server drive. First, go to **Add Track | Add Track From Server File**.

![add_server_png](images/add_server.png)

## Adding BAM Files As Single Tracks

In the *Specify Track Source* window, select **Alignment track | Sorted BAM file**.

![specify_server_track_png](images/specify_server_track.png)

Choose the two BAM files, *SRR064173.subset.bam* (RNA-Seq alignment) and *SRR521462.subset.bam* (DNA-Seq alignment). Click **Open**.

![image15_png](images/image15.png)

The two new BAM tracks will appear at the bottom of the browser. The first time that tracks are added, it may take a few minutes while indexing is performed. This only occurs once.  

The user can zoom in and out using the mouse wheel or zoom tool at the top right of the tool bar.

![image16_png](images/image16.png)

We can navigate to a gene region by typing a gene symbol, e.g. *abl1*, in the search box (on the top-left corner, arrow). The coverage will be displayed in red in exon region and blue in intron/intergenic regions.

![abl_search_png](images/abl_search.png)

## Adding BAM Files As Combined Tracks

The user can choose to merge multiple BAM files into a single track. In the Specify Track Source window, select **Alignment track | multiple sorted BAM files**.

![add_combined_png](images/add_combined.png)

Choose the four fusion BAM files and click **Open**.

![image19_png](images/image19.png)

A new track from four BAM files is created in Genome Browser:

![abl1_all_png](images/abl1_all.png)
