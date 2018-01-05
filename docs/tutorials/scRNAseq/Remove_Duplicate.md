# Remove Duplicate

**This module is optional for this tutorial, user can run this or just skip this part, and jump to the step for Quantification.** Remove Duplicate can be used to remove duplication for Single Cell Bam files. The module will be useful if the user wants to have a clean (duplicate removed) BAM file for downstream analysis.

To access this module, user can go to **Analysis | NGS | Single Cell RNA-Seq | Remove Duplicates**:

![RemoveDuplicate](images/Remove_Duplicate.png)

Use the default options and just input the Output name and output folder, then click **Send To Queue** to submit this job:

![RemoveDuplicate4SCData](images/Remove_Duplicate_for_scData.png)

Once this job is finished, user should be able to see a new NgsData object in Array Studio GUI, as well as new BAM files in the specified output folder:

![RemoveDuplicateOutput](images/Remove_Duplicate_output.png)
