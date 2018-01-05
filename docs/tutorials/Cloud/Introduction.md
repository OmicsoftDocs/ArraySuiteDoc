# Introduction

## Omicsoft Cloud
Studio/Server On Cloud is OmicSoft's solution to manage and analyze large Omics data using cloud computing. The standalone edition of Array Studio on the Cloud allows you to seamlessly run all Array Studio analytics from Amazon, combining the storage of S3 with the analytical power of EC2. Easily scale up any number of instances for every analysis. Array Server with Cloud will handle security credentials on server and submit/manage cloud files/jobs as seamlessly as running on ArrayServer.

This tutorial only covers the Array Studio on the Cloud. For Server on Cloud, please read "Server Analysis (Basics)" tutorial.

## Array Studio on the Cloud

Array Studio on the Cloud is a cloud solution, allowing users to store, share, search, and integrate their microarray/SNP/CNV/NGS projects and data. The users can easily share analyzed data with clients and colleagues. Cloud computing can remove the limitation of on-site computing capacity and dramatically improve computing efficacy. Array Studio can handle:

*   pinning up the correct number of instances

*   Accessing the data from S3

*   Running the analysis with the optimal EC2 configuration (storage, memory, and CPUs)

*   Spinning down the instances

*   Storing the generated data back on S3

*   Genome browser integration with S3

Cloud-based analysis allows the user to run jobs on cloud, which usually has more computing power than a desktop computer. The Array Studio client software, installed on a local desktop machine, is used to interact with the cloud.
Tasks such as job submission, monitoring, file transfer and data visualization can be done through the client software.

All the Array Studio modules available for local analysis are also accessible for
could-based analysis. The graphic interfaces are almost the same.

## Cloud Project

A "Cloud Project" is a project that is created on the cloud, rather than on the user’s client machine. This project is cached locally on the client machine, in case of loss of connection to the cloud, but is automatically updated each time the user logs in or clicks the save button. The cache is stored in the user’s home folder, typically My Documents/Omicsoft/Cloud Projects?. A Server Project, when stored locally in the cache folder, has a different filename suffix (.oscprj) as compared to a regular project (.osprj) and can only be opened when the user is connected to the cloud.

The concept behind the Cloud Project is that any data that is added to a project, must first be stored on the cloud. When the user adds a new dataset (whether it be Gene Expression, CNV, or NextGen sequencing), they will be prompted with the folder structure of the Array Studio on Cloud instead of their local file system. If the user wishes to use a file from their local file system, they must first upload the file to the cloud file system.

All data addition and extraction is done on the cloud, instead of the users client machine. It allows the user to use the power of the cloud, instead of their individual client machine for the importing of data. This is extremely important for some memory/cpu intensive importing operations (such as alignment of a fastq file to the genome for NextGen sequencing data). After data extraction, alignment or data summarization, minimal data will be downloaded to the client machine, where the user can add views, run additional statistical analysis, etc.

## Test Dataset

In this tutorial, we will show how to create a cloud project for cloud-based analysis. To demonstrate, we will use the same dataset for server testing to test cloud. The user should first download the demo data file for use in the tutorial and save it to the local machine. The file can be access from [here](http://omicsoft.com/downloads/data/tutorial/ServerBasics.zip)
