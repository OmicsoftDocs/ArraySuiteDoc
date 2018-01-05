# Add Expression and Comparison Data to Land

After you have successfully created **.alv** and **.tlv** files containing your expression and comparison data, respectively, you can add these data to an existing or new ArrayLand.

## Create a New Land

If these data will be added to a new Land, you must create this Land first.

Connect to Array Server with administrator privileges, then click on the **Land** tab:

![ArrayStudio_Tabs](images/ArrayStudio_Tabs.png)

Switch to the **Land** tab, then click **Tools | Create Land**:

![CreateLand_Menu](images/CreateLand_Menu.png)

In the window, give your Land a unique name for the server, and enter additional settings:

![CreateLand_Window](images/CreateLand_Window.png)

In the tutorial data set, you will find a file "TutorialLandSettings.cfg" that contains some basic settings.

When successful, you will get the following message:

![CreateLand_Success](images/CreateLand_Success.png)

## Add Sample and Project MetaData to Land

Before you add your actual data to your new Land, you can add the Sample and Project MetaData.

In the tutorial dataset, the Sample Metadata are in "Brawndocin_Slurmycin.V2.Expression.Design.txt", and the Project Metadata are in "Brawndocin_Slurmycin.V2.ProjectMetaFile.txt".

In the **Land** tab, click **Manage | Samples | Manage Sample Meta Data** or **Manage Project Meta Data**:

![ManageMetaData_Menu](images/ManageMetaData_Menu.png)

In the **Sample Metadata** and **Project Metadata** windows, you can add, replace, clear, and remove metadata for samples.

To add new sample metadata, click **Add/Replace**, and navigate to the Sample Metadata file.

If properly imported, the window will look similar to this:

![SampleMetaData_Window_Imported](images/SampleMetaData_Window_Imported.png)

You should also import the project metadata file, which should result in a window like this:

![ProjectMetaData_Window_Imported](images/ProjectMetaData_Window_Imported.png)

## Add .alv and .tlv files to server

If you are processing the tutorial data, you will have generated 6 .tlv files (one per comparison between sample groups) and 56 .alv files (one per sample).

Upload these to your Array Server, by clicking on the **Server** tab, then clicking **Server File | Browse Files**:

![BrowseFiles_Menu](images/BrowseFiles_Menu.png)

Navigate to a location to store your files, and click **Upload**:

![BrowseFiles_Window](images/BrowseFiles_Window.png)

Navigate to your .alv and .tlv files, and upload them to the server.

Now switch back to the **Land** tab, and click **Tools | Publish To Land**:

![PublishToLand_Menu](images/PublishToLand_Menu.png)

Navigate to your server files and click *Send To Queue*:

![PublishToLand_Window](images/PublishToLand_Window.png)

 Note: You can only publish data one job at a time, so if you have submitted a set of files to the server for publishing, you must wait for that job to complete before submitting the next job.

When all of your .alv and .tlv data have been published, the ServerJobs queue will say "Finished", and you can start exploring your Land.
