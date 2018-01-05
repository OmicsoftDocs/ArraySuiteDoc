# Land Tools

ArrayLand provides other Tools to download a slice of Land to ArrayStudio local analysis:

![NewImage103_png](images/201510-103.png)

##Download Sample Data To Local Analysis

The **Download Sample Data To Local Analysis** function allows users to query the Land database with a list of genes or a list of samples and download them as OmicData/Table to Local Analysis project.

Users must first open or create a project in ArrayStudio Analysis:

![image79_png](images/image79.png)

Then open the **Download Sample Data To Local Analysis** window in the **Land** tab. There are two options. Users can download selected genes across all samples, and can also download selected samples across all genes. Specify the target ArrayStudio project to store downloaded Land data, a collection of samples (sampleSet) or get all samples. Choose the land data type to download, each one will be an OmicData/Table in ArrayStudio project. Note:

- **Original data** is the original values stored in Land, such as RNA-Seq FRKM at transcript level and microarray data at probeset level.
- **Gene level** data are values summarized at gene level.
- **Matrix data** is to organize output as *feature by Samples* in "MicroArray" format if possible.
- By default, only *PrimaryGrouping* and *SecondaryGrouping* columns are attached as design in each generated OmicData. Check **Full meta data** box will be download all sample meta data as a table in the project.

![NewImage88_png](images/201510-88.png)

Downloaded data are shown as project contents:

![image81_png](images/image81.png)

User can do more advanced data analysis and visualizations on downloaded data objects use ArrayStudio functions.

## Download Sample Data To Text Files

User can also download land data to text files through **Land | Download | Download Sample Data To Text Files**:

![NewImage89_png](images/201510-89.png)

![image83_png](images/image83.png)
