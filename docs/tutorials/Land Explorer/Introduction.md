# Introduction

**Note to reader**: The tutorial pages are actively being written to describe the usage of the Land Explorer and the recent 2018Q2 release. Please check back for updates or e-mail support@omicsoft.com if you have specific questions not addressed here.

## Land Explorer

OmicSoft uses ArrayLand framework to deliver large amounts of clinical and "omic"-data to biologists with simplistic visualization. ***Land Explorer*** is the quickest way to explore OmicSoft Land data (OncoLand, DiseaseLand, and Internal Lands). Users of Array Studio may be familiar with the content provided within the Land Explorer framework. The streamlined web interface uses our most popular visualizations to help researchers and clinicians explore OmicSoft Lands.

### Video introduction to Land Explorer

Please see our video for a basic introduction to Land Explorer:

<div class="video-wrapper">
  <iframe width="1280" height="720" src="https://www.youtube.com/embed/CYu4QVXCKOc" frameborder="0" allowfullscreen></iframe>
</div>

Land Explorer is hosted on a Windows machine which connects to ArrayServer to provide access to rich visualization of Omic-data, directly in a user's web browser, meaning no extra software required. Land Explorer can by used as a companion product to OmicSoft's ArraySuite (to use with internal Lands and OmicSoft Lands), or as a standalone product hosted by QIAGEN/OmicSoft. Like ArraySuite, Land Explorer is fully customizable to meet the needs of its users.

These tutorial pages demonstrate the utility of Land Explorer, including a description of the many [views](./Land Views/Views.md) available, as well as the [general usage and customizations](./Using Land Explorer/LandExplorerInterface.md) of these views.

## Land Explorer usage

Users can login to Land Explorer using their ArrayServer credentials. Please contact your ArrayServer adminstrator or support@omicsoft.com if you are having issues logging in. Once you connect to the LandExplorer, there are two options for a landing page that can be customized for each LandExplorer installation: An Optional FrontPage or a Land View.

### FrontPage Option

This option allows users to query data across all Lands related to specific Sample Types. For example, the view below shows a distribution of all samples represented with the OncoLand, DiseaseLand, BodyMap, Cell Line and Single Cell collections, including sample counts, counts of data types and how these samples are distributed across all Lands.


For more information on how the FrontPages are configured and used, please visit the FrontPage [help](./FrontPage/FrontPage.md) menu.

![Front_Page](images/FrontPageNirav.png)

### Land View Option

If a FrontPage option is not defined in Land Explorer, the default view will be a Land View. In this view, the default land chosen by the administrator (TCGA by default) will appear. Users can switch to other Lands by simply clicking **Select Land**:

![LandPortal_login_png](images/LandPortal_login.png)

The default **TCGA_B37 Land Explorer** view shows a histogram plot of samples grouped on the y-axis by Tumor Type, and colored on the x-axis by Sample Type. Other views are also available for users to query the sample data at a general level.
