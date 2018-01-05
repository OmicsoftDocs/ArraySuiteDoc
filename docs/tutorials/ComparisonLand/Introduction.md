# Introduction

## ArrayStudio

Array Studio runs local NGS analysis in 64-bit mode on a Windows 64-bit computer with at least 8GB of RAM. Server-based analysis allows the user to run jobs on a remote server (Linux or Windows), which usually has more computing power than a desktop computer. This tutorial is based on local microarray analysis using a Windows Workstation with 3.4GHz Intel® Core TM i7-6700 Processor (# of cores: 4; # of threads: 8) with 24GB RAM. The tutorial dataset is small and does not require these hardware specifications; However, processing of large numbers of whole-transcriptome table data, with thousands of samples and comparisons, can be memory-intensive.

It is highly recommend that the user complete the prerequisite for this tutorial: **the Microarray tutorial**, as a way to learn the basics in Array Studio.

This tutorial assumes minimal working knowledge of Array Studio. However, an understanding of Array Studio data types, as well as the Views and Analysis modules within ArrayLands, will significantly improve your custom ComparisonLand design.

This tutorial also assumes a basic understanding of absolute and relative file paths, for editing .oscript files to find files on your local computer.

## Test Dataset

This ComparisonLand tutorial will cover the importing and analysis of a small synthetic dataset of microarray expression, from 7 sample groups (56 samples).

A .zip file containing all required text files for this analysis can be found at the following URL:

http://omicsoft.com/downloads/data/Tutorial/Help/ComparisonLand.Tutorial.zip

simply unzip this file into a local folder, and proceed with the tutorial.
