# Convert Inference Data to .TLV

If you have statistical inference data for your expression data, such as fold-change and P-value calculations,
you can convert these into ComparisonLand-compatible **.tlv** files.

You can also calculate statistical inferences using multiple modules within Array Studio, including DESeq, ANOVA and General Linear Model.

##Formatting the Comparison Data File

For this tutorial, the expression data were tested by One-Way ANOVA of the six treatment sample groups (Brawndocin at 0.3, 1, 3.3, and 10uM,
and Slurmycin at 1 and 10uM) compared to a common group of vehicle samples.

The resulting inference table was converted to the following tab-delimited format:

![ComparisonDataFileFormat](images/ComparisonDataFileFormat.png)

The first column should be the probeset/GeneID. Subsequent columns should be in the following order:

* *treat1*.log2FC
* *treat1*.rawPValue
* *treat1*.adjPValue
* *treat1*.caseMean
* *treat1*.controlMean
* *treat2*.log2FC
* *treat2*.rawPValue
* ...
* *treat100*.adjPValue
* *treat100*.caseMean
* *treat100*.controlMean

The full file for this tutorial is "Brawndocin_Slurmycin.V2.Comparison.Data.txt".

Each row should contain all comparisons for a single gene/probeset.

Also, each *treat* name should be unique among the entire dataset.

Once you have converted your inference data into the proper format, you can proceed to formatting the *comparison metadata* file.

## Formatting the Comparison Metadata file

The **Comparison Metadata** file is a tab-delimited file that contains the information that groups together all of the samples (in the .alv files), extracts sample metadata for filtering/grouping of comparisons, adds additional comparison metadata, and connects these to the **Comparison Data** that you prepared in the previous section.

Thus, it is essentially that you carefully plan the metadata that should be included in your comparisons.

The minimum data for the **Comparison Metadata** file are as follows:

* **ComparisonName**: This should be the first column, and the names in this column should match the comparisonNames in your **Comparison Data** file (without ".log2FC", "PValue", etc).

* **MetaColumns**: A list of **Sample Metadata** column names, indicating the metadata to include in the comparison metadata.

    - "Treatment","CellType", and "Tissue" **Must** be included in this column (and as columns in the **Sample Metadata** file).

    - "DiseaseCategory" is not absolutely required, but some Views group samples by this column, so will not work properly without this column.

    - Any additional **Sample Metadata** columns that are included must be consistent within a sample group. For example, if your **Case** samples include both HCC4006 and HCC827 cells in the **CellLine** column, you cannot include **CellLine** in your Comparison metadata.

* **CaseSampleIDs**: A delimited (',' or ';') list of Sample IDs included in this comparison, matching your **Sample Metadata** files Sample IDs.

* **ControlSampleIDs**: A delimited (',' or ';') list of Sample IDs included in this comparison, matching your **Sample Metadata** files Sample IDs.

* **TestCategory**: A description of the type of comparison being made.

    - Standard Test Categories include "Disease vs. Normal", "Treatment vs. Control", "Treatment1 vs Treatment2", "Tissue1 vs. Tissue2", "Responder vs. Non-Responder", "Disease vs. Normal", "Disease1 vs. Disease2", "CellType1 vs. CellType2", and "Other Comparisons".

* **TlvID**: A unique name for your comparison (i.e. unique across your entire ComparisonLand, not just the project).

* **ProjectName**: A name that groups the set of comparisons.

* **PlatformName**: A description of the source NGS or Microarray platform.

* **ComparisonSoftware**: The name of the software that calculated the inferences, such as "DEseq" or "limma"

* **StatsModel**: A description of the statistical model.

* **SampleDataMode**: A description of the type of underlying measured data, such as "Expression_Intensity_Probes" or "RnaSeq_Transcript".

Please see the tutorial file "Brawndocin_Slurmycin.Comparison.MetaFile.txt" for a properly-formatted example.

## Running the Oscript to Convert Inference data to Tlv

Once you have formatted your comparison data and metadata files, you should edit the **Oscript** file to specify the input locations for the following files:

* Comparison Data File (Brawndocin_Slurmycin.V2.Comparison.Data.txt).

* Comparison MetaData File (Brawndocin_Slurmycin.V2.Comparison.MetaFile.txt).

* Sample MetaData File (Brawndocin_Slurmycin.Expression.Design.txt).

Also, specify the output location for the **.tlv** files.

The following **Oscript** file can be found as "ExtractExternalInferenceReport.oscript": ::

	 Begin ComparisonLandTools /Namespace=NgsLib;
	 Files "";
	 Reference Human.B37.3;
	 GeneModel OmicsoftGene20130723;      
	 Options
	 /Action=ExtractExternalInferenceReport
	 /ComparisonDataFile=
	 "Z:\Users\Joe\Tutorial\ComparisonLand\Final\
	 InputFiles\Brawndocin_Slurmycin.V2.Comparison.Data.txt"
	 /SampleMetaDataFile=
	 "Z:\Users\Joe\Tutorial\ComparisonLand\Final\
	 InputFiles\Brawndocin_Slurmycin.V2.Expression.Design.txt"
	 /ComparisonMetaFile=
	 "Z:\Users\Joe\Tutorial\ComparisonLand\Final\
	 InputFiles\Brawndocin_Slurmycin.V2.Comparison.MetaFile.txt"
	 /OutputFolder=
	 "Z:\Users\Joe\Tutorial\ComparisonLand\Final\TLV"
	 /MappingID="Affymetrix.HT_HG-U133A_Human.B37.3" ;
	 End;

Update the **oscript** paths to indicate where the files are located on your local computer, then run the **Oscript** as before in **Array Studio**, and check that the **.tlv** files have been generated in the specified folder:

![TLV_Output](images/TLV_Output.png)
