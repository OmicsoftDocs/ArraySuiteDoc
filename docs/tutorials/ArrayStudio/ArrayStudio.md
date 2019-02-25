##Introduction

###What is Array Studio?
Array Studio is a software package that provides state of the art statistics and visualization for the analysis of high dimensional quantification data (e.g. Microarray or RT-PCR/Taqman data), genotype data (e.g. SNP or Copy Number data) and Next Generation Sequencing data. It provides the fastest, easiest and most powerful solution for "-omic" and "NGS" data analysis on the market. More than 400 features have been implemented based on feedback provided by industrial and academic users.

**Features**

- Array Studio includes over 40 unique views, all of which are fully interactive (e.g. selection, zoom, etc.) and highly customizable (e.g. change axis, colors, shapes, etc.). Most of these views also have trellis support. All the views can be exported as images or PowerPoint slides by a single mouse click.
- More than 50 analytical modules were designed for ease of use so that biologists can function at near the level of informatics specialists. The high dimensional linear modeling module provides the complete statistical analysis for multiple ANOVA, ANCOVA, repeated measure, split plot and a variety of other experimental designs. Non-negative matrix factorization and spectral map analysis are two of the many data exploration modules in the software. Data mining modules provide comprehensive support for classification (e.g. SVM and KNN) and regression (e.g. LASSO and Neural Network), with built-in variable selection and honest cross validation. Takes seconds or minutes instead of hours to do an analysis on a regular laptop computer!
- Array Studio also provides comprehensive support for project management, data manipulation, quality control, pathway analysis, gene ontology analysis, and power analysis. For industrial users, an internal audit trail and scripting are useful for data integration and customized analysis pipeline. Array Studio will automatically save all analysis logs to text file and provide a link to this file  in the "Audit Trail Description" tab.
- Array Studio integrates with Array Server, Omicsoft's enterprise solution for Microarray/CNV/SNP/NGS data storage, search and integration.  Easily retrieve projects from Array Server, and/or publish back to the server for storage and searching purposes.

**Benefits**

- Fastest data analysis and visualization on the market
- General linear model benchmarked with SAS
- Automatic project management, annotation support and script generation
- One-Click exporting of tables to Excel and all visualizations to PowerPoint
- One-Click downloading of data from the Gene Expression Omnibus (GEO) website, including the ability to automatically parse both design (sample information) and annotation, so that the project is immediately in the correct form for further analysis and visualization.
- One-Click downloading of data from the Sequence Read Archive (SRA) website, including the ability to automatically convert sra files into fastq files.
- VariableView, for looking at expression values on a per-gene basis
- General Linear Model for performing complicated analysis, including the ability to analyze mixed models, continuous and class covariates, nested factors, etc.
- Quality Control Modules, including generating Correlation Heatmap, Kernel density views, Principal Component Analysis, and more.
- Stunning performance: Most modules in Array Studio take seconds, not minutes to run. Array Studio has been shown to handle 20,000 samples and millions of rows on an average laptop computer. A top-tier workstation is not necessary to run Array Studio effectively.
- Interactive GenomeView and RegionView for visualizing CNV segmentation results.
- Ability to easily import 1000s of microarray, SNP, or CNV chips on a regular computer
- Fast and powerful segmentation algorithm for Copy Number analysis. GenomeView allows easy editing of copy number segments, as well as visualization of segments in relationship to Log2Ratio and AlleleDifference (B Allele Frequency)
- The Taqman/RT-PCR Import and Normalization wizard is industry leading. The module was designed for use by top statisticians and bioinformaticians at a leading pharmaceutical company, and includes the ability to import directly from ABI Result Text files, normalize the data using a number of statistical methods, and visualize the results using the same visualizations used elsewhere in Array Studio.
- Comprehensive statistical support for SNP, Genotyping, and Copy Number analysis, including the analysis of basic association studies, quantitative traits, categorical traits, survival trait analysis, repeated measure traits, Linkage disequilibrium analysis, Dose data association, probability association analysis, and more.
- Automatic annotation support and built-in annotation browser-For most leading microarray and genetic products, Array Studio automatically downloads gene annotation and links it to every dataset and result created by users. Web Details on Demand allows users to quickly link to public resources that relate to selected probe sets or markers in a dataset.
- Single deployment with automatic update support ensures that users will always be running the latest version. With Omicsoft's commitment to implementing reasonable user requests, this allows users to always have the newest software, including any and all modules released since users purchased the software.
- NGS workflows for DNA-seq, RNA-seq and miRNA-seq. The workflows include our high performance alignment modules (works for both single end and paired end) and many downstream analysis. For oncology users, we also developed the full gene fusion modules for both single-end and paired end modes. Papers and white papers on NGS are available upon request for existing users.

Array Studio provides an integrated environment for analyzing and visualizing high-dimensional data.  It is convenient for organizing and visualizing data with its Solution Explorer, which organizes each project into two main sections (-Omic data and Table data), as well as different folders:, QC, Inference, List, Cluster, Text, Attachments and other categories.  The Solution Explorer can contain multiple projects, and data can be shared among projects.  Each view is controlled by a View Controller, which performs view customization, applies filtering, and displays legends; Furthermore, its interactive visualization technique provides the details of data with the Details Window and the Web Details Window.

##Installation

###Requirements
Array Studio requires Microsoft .NET 3.5 framework.  As a result, most versions of Array Studio require that users have administrative privileges to install .NET 3.5 Framework, or the ability to do so before installing Array Studio. By default, the installation page for Array Studio will automatically install .NET 3.5 Framework if users do not have this installed previously.

While Array Studio does not have any specific requirements for memory or processor speed, it is recommended that users have at least 1gb of RAM for microarray analysis, and at least 2gb of RAM for ExonArray, SNP/Genotyping, and CNV analysis.

For microarray analysis, hard drive space is not an issue, however users should ensure that they have sufficient hard drive space for larger ExonArray, SNP/Genotyping, and CNV analysis.  Extremely large datasets, such as Dose or Probability SNP data, utilize a large amount of hard drive space. The user should ensure that there is sufficient space on the hard drive for such analyses.

For NGS analysis in 64-bit mode 8 GB of RAM is recommended, for 32-bit mode 2 GB of RAM is recommended. For hard drive space, both your Omicsoft temp folder and the data for the analysis must reside on a hard drive that has 3-times the amount of free space as the size of the raw data files.

The Omicsoft software home directory is typically located in users' My Documents folder, under the Omicsoft folder.  This folder contains all of users' annotations, favorites, Ontology, Refseq, Ensembl, Hapmap data, and more.  In addition, this folder is used as the temporary working directory.  If users are concerned about space on the hard drive containing this folder, the *Omicsoft home directory* can be changed by going to  **Tools  | Preferences | Advanced | Omicsoft**.

###Installing Array Studio
Bioinformatics is a fast evolving field. We are developing new analysis functions and options every day. The software is updated frequently. We do have a stable Array Studio version 10.0. Please contact omicsoft.support@qiagen.com if you wish to use the stable version for data analysis.

ArrayStudio can be installed/launched using ArrayStudio Launcher. Launcher is installed through ClickOnce deployment. On an an internet-connected computer, open the following link in
Internet Explorer, click install in the page below:

http://omicsoft.com/software/ArrayStudioLauncher/publish.htm

It will create a desktop icon "ArrayStudio Launcher". User can then click the icon and launch ArrayStudio regardless which default internet browser has been set on your computer. The Launcher will check whether there is any software update available and ask user to decide whether to update studio or not.

###Array Studio GUI
When Array Studio is first installed, it will look similar to below.
If you have previously opened projects in Array Studio, you will see the Last Opened Projects window.  If so, just click **cancel** so that Array Studio looks similar to below.

Notice at the top there will be four tabs: Analysis, Server, Land, and Browser.

![ArrayStudioGUI](images/ArrayStudioGUI.png)
