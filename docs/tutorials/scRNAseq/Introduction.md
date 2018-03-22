# Introduction

## ArrayStudio

Array Studio runs local NGS analysis in 64-bit mode on a Windows 64-bit computer with at least 8GB of RAM. Server-based analysis allows the user to run jobs on a remote server (Linux or Windows), which usually has more computing power than a desktop computer.
This tutorial is based on local NGS analysis using a Windows Workstation with (Window 10 Pro) with 3.60GHz Intel® Core TM i7-4790 Processor (# of cores: 4; # of threads: 8) with 16GB RAM.

It is highly recommend that the user complete the prerequisite for this tutorial:
**the Microarray tutorial**, as a way to learn the basics in Array Studio. This tutorial assumes working knowledge of Array Studio, standard visualizations, and different modules within the software. As many of the downstream data types from next generation sequencing are "Microarray" datasets, the Microarray tutorial is an invaluable starting tool.

## Test Dataset

This Single Cell RNA-Seq (scRNA-Seq) tutorial will cover the importing and some analysis of a public dataset. This dataset can be accessed from NCBI GEO database: [GEO GSE85241](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE85241) which was run on the Illumina NextSeq 500(GPL18573) platform, and adopting the method of CEL-Seq2. There are 32 samples in total and each sample has 2 fastq files as input, as it’s paired-end sequencing data.

As described in the document (GSE85241_readme_demultiplexing_Cel-seq_data.pdf) downloaded from GEO database, read 1 should be parsed in the following manner: “the first 8 basepairs are the Cel-Seq cell barcodes (see list at the bottom of the same document). The following four basepairs are random basepairs of the unique molecular identifier, which can be used to count individual molecules for each transcript. The rest of read 1 consists of mostly polyT and is not used. Read two is then mapped to the reference genome of choice (hg19 in our case).”

Based on this description, in this tutorial we will extract the cell barcode and UMI information from read1, then align read2 to human genome, and perform downstream quantification and clustering analysis.

If users are interested in testing with this project, the data can be downloaded from NCBI: [SRP080991](https://trace.ncbi.nlm.nih.gov/Traces/study/?acc=SRP080991), or using our GUI for downloading SRA to download the fastq files: [Download SRA in ArrayStudio](http://www.arrayserver.com/wiki/index.php?title=DownloadSRAData.pdf).
After retrieving these data, you can begin the tutorial.
