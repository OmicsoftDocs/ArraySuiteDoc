# Genome Browser Visualization

Processed data from CNV analyses performed in this tutorial can also be viewed directly in the Genome Broswer tab. To access the browser, simply click the **Browser** tab at the top of your screen:

![genome_menu_png](images/genome_menu.png)

If you have not already done so, create a New Genome Browser by clicking new. You will see the following prompt:

![new_genome_browser_png](images/new_genome_browser.png)

Choose the default reference and gene models and select and output folder and name. Click "OK". Go to **Add Track | Add Track from Analysis**:

![add_track_png](images/add_track.png)

First, try choosing the option *Segment track: segment data* and click "OK".

![segment_data_png](images/segment_data.png)

Find your open segment table from this tutorial and click "OK":

![segment_data2_png](images/segment_data2.png)

Choose the default options and click "OK" again:

![segment_default_png](images/segment_default.png)

You will see two additional tracks appear in your **Genome Browser**: *Log2RatioMean* and *CNStatus*. Browse to chromosome 13 within the toolbar and notice that the *Beta2* sample we examined earlier has a *log2RatioMean* of ~0.35 and a corresponding copy number status of 3 for a large portion of the chromosome:

![genome_view_png](images/genome_view.png)

User can zoom in on regions of interest by using magnification tools in the upper right part of the browser, the click wheel of a mouse, or by simply holding *Shift* and left-clicking to highlight a region.

In addition to the segment tracks, one can upload additional CNV tracks. Go to **Add Track | Add Track from Analysis**:

![add_track_png](images/add_track.png)

This time, choose the option *Numeric track with multiple series: CNV data*:

![cnv_data_genome_browser_png](images/cnv_data_genome_browser.png)

Find your CNV analysis output and click **OK**. Select the data you want to visualize and click **OK**. Here, we choose all the data and set all other parameters to default:

![choose_output_png](images/choose_output.png)

In this view you can visualize the individual SNPs on the CNV chip and their position within the genome. This can also be achieved by going to the Table view of the CNV data, right-clicking on individual SNPs, and selecting the genome browser view:

![table_to_genome_png](images/table_to_genome.png)

As you can see with this SNP, our top sample, has an elevated log2 value relative to the other samples. Users are encouraged to explore display options to adjust track height, width of data points, and more:

![chosen_snp_png](images/chosen_snp.png)
