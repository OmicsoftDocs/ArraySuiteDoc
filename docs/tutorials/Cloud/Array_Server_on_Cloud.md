# Array Server on Cloud

The user can also run server jobs on cloud.
This tutorial is drafted for standard users. For how-to configure Server with Cloud, please contact Omicsoft Support to get the manual for Server on Cloud admin.
After ArrayServer admin configured the Server with Cloud, standard users do not need to set up Cloud Preferences but only need to connect to the server with cloud integration through **Server** tab:

![image20_png](images/image20.png)

When connected, the window looks the same as the server window:

Notice that the **Cloud** tab will not appear.

![image21_png](images/image21.png)

## Uploading Files to server cloud

To run server jobs on cloud, the users should upload the data files on specific cloud folder that assigned in advance. Go to **Server File | Browse Files** window:

![image22_png](images/image22.png)

Then go to the **cloud folder** configured in advance. Please contact the admin person if the user does not
know where the folder is configured as Cloud folder. In the folder, the users can create their own folder and upload the data the same way as running a server project:

![image23_png](images/image23.png)

## Run server project on cloud

To run server project on cloud, make sure that you already upload your files to the cloud folder. Please create a server project in **Analysis** tab first. The analysis window and analysis steps are same as running a server project. When adding data to project, remember to browse the right cloud folder for your files:

![image24_png](images/image24.png)

After sending the data to queue, the job progress could be monitored the same way as server project:

![image25_png](images/image25.png)

## Run multiple jobs on cloud

When running multiple jobs (For example, multiple samples sequencing data alignment), multiple cloud instances will be allocated. This makes it much faster to perform the analyses.

To test this, please download the RNA-seq demo dataset from:

[^link^](http://omicsoft.com/downloads/data/tutorial/RNASeq.zip )

More detailed description of the dataset can be found in RNA-Seq Analysis Tutorial.

For illustration purpose, we will only use two samples to reduce the process time. Again, remember to go to the right cloud folder to load the data:

![image26_png](images/image26.png)

![image27_png](images/image27.png)

The demo dataset is paired-end sequencing data; please check the **Reads are paired** check box.

For Server project to run on cloud, the users must specify output folder. The directory should be under the cloud folder.

Upon job submission, again, the job could be monitored:

![image28_png](images/image28.png)

The users can right click on the job and select **View Full Log**:

![image29_png](images/image29.png)

In the *Log* window, as you can see, the jobs are being submitted to cloud NGS instances, 2 cloud instances will be started as we have two samples to align:

![image30_png](images/image30.png)

As a general user, you cannot monitor the Cloud Instances for Server Cloud this time.

The users could go back to Analysis tab and continue any downstream analyses and visualization:

![image31_png](images/image31.png)

Congratulations! Now you can successfully run server project on cloud!
