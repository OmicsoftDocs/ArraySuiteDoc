# Integration

## Pipeline Integration

### Pipeline Scripts

User can run a pre-configured pipeline on a sample set. Pipeline can be as simple as raw data QC, alignment and then do quantification analysis on NGS data. Pipeline scripts are managed by ArrayServer administrators in **Server | Manage | Manage Scripts**:

![image17_png](images/image17.png)

![image18_png](images/image18.png)

### Run Pipeline Script in Analysis

To run a pipeline on a SampleSet, open or create a server project in the **Analysis** tab. Then go to **Add Data | Add Data From Server**:

![image19_png](images/image19.png)

Select a SampleSet

![image20_png](images/image20.png)

Select a pipeline script:

![image21_png](images/image21.png)

Fill required parameter values and click **OK** to run:

![image22_png](images/image22.png)

### Run Pipeline Script during Sample Registration

User can run pipeline script during sample registration process by adding **[Pipeline]** section in sample registration file.

![image23_png](images/image23.png)

By using the sample registration file above, a server job will be submitted at the end of sample registration to create a server project with ID *TutorialRNASeq1*, using pipeline script *Tutorial.RNASeq.v1.pscript* and specified parameter values.

## Genome Browser Integration

As we mentioned above, sample registration supports multiple file formats, including BAM (NGS alignment) files. User can modify the old registration file, adding a file path to BAM files:

![image24_png](images/image24.png)

Registering this file (**Server Sample | Register Samples**) will update samples with BAM path.

![image25_png](images/image25.png)

Now, the alignment files (BAM files) of samples can be loaded in the Genome Browser tab directly through **Add Track | Add Track From Server Samples**:

![image26_png](images/image26.png)

User can add individual samples or the whole sample set. Here we choose the *TutorialRNASeq.fullData* sampleset:

![image27_png](images/image27.png)

User has the option to add one sample as one genome browser track:

![image28_png](images/image28.png)

Or create tracks for groups defined by sample registration meta data:

![image29_png](images/image29.png)

Choose *Cellline* as group which will create two genome browser tracks: K562 and MCF7.

![image30_png](images/image30.png)

User can split the combined tracks to individual samples by right click and select **Split Into Multiple Tracks**:

![image31_png](images/image31.png)

For more information and features available in the genome browser, please read the **Genome Browser Tutorial**.
