# Introduction

## Genome Browser

OmicSoft's Genome Browser is fully integrated with Omicsoft's Array Suite package (Array Server and Array Studio). The Genome Browser tab can be found in Array Studio and Array Viewer software:

![image9_png](images/image9.png)

The OmicSoft Genome Browser can visualize NGS data in 32-bit mode on a Windows 32-bit computer with 2GB of RAM minimum, or in 64-bit mode on a Windows 64-bit computer with 8GB of RAM.
64-bit mode can run much faster than 32-bit mode, and is highly recommended when there is no Array Server connection and alignment files are not indexed.

It is highly recommended that the users complete the prerequisite for this tutorial: RNA-Seq and DNA-Seq tutorial, as a way to learn the basics in sequencing data analysis.

## Test Dataset

This Genome Browser tutorial will cover the importing and visualizing six NGS alignment files generated from RNA-Seq and DNA-Seq tutorial.

| Sample ID          | Description                                                    |
|:-------------------|:---------------------------------------------------------------|
| SRR064173.subset   | DNA-Seq alignment BAM                                          |
| SRR064173.FusionSE | DNA fusion junction spanning reads detected by ArrayStudio     |
| SRR064173.FusionPE | DNA inter gene fusion read pairs detected by ArrayStudio       |
| SRR521462.subset   | RNA-Seq alignment BAM                                          |
| SRR521462.FusionSE | RNA fusion junction spanning reads detected by ArrayStudio     |
| SRR521462.FusionPE | RNA inter transcript fusion read pairs detected by ArrayStudio |

To minimize the file size, we provide a subset of the alignment files containing regions of four genes: BCR, ABL1, NUP214 and XKR3:
[^link^](http://omicsoft.com/downloads/data/tutorial/GenomeBrowser.zip )

This tutorial mainly focuses on browsing next generation sequencing data and its integration with the analytical tools of Array Studio.
For more details on general functions and usage of the Genome Browser, please refer to the Genome Browser online help:
[^link^](http://www.arrayserver.com/wiki/index.php?title=GenomeBrowser_Online_Help )
