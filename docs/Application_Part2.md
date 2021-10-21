---
layout: default
title: Identify and Acquire Data
parent: Application
nav_order: 2
---

# Acquire Data

## Project Folder

I've gotten the ball rolling for you and setup a project.  Download the [Module5 folder here]().  This project contains two layers: a DEM for the Port Alberni area and a vector layer representing the coastline.  It also contains a model that you can use identify areas at risk for Tsunami inundation.  Your task will be to incorporate data from the City of Port Alberni, the Province of British Columbia, and Statistics Canada.  Download the [PA_Data.zip]() and extract it to your Module5 folder.  This folder contains Properties.shp (properties in the city by zoning type) which you should import into the PA_Risk_Assessment_Inputs feature dataset.  This folder also contains two text files:  ZoningCodes is metadata for Properties.shp.  We don't need to worry about it for now.  Shelters.csv is a text file with the Lat/Lon coordinates of the tsunami shelters.  See the video below for instructions on how to import point data from text files so you can import the Shelters layer into the PA_Risk_Assessment_Inputs feature dataset.

<iframe width="560" height="315" src="https://www.youtube.com/embed/KTZ5ix_O8Wo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### QA

Why do we use a feature dataset to hold all our input layers?

A) No reason
B) So everything is neatly grouped in one folder
C) To ensure all our vector data is in the same projection, the feature dataset will automatically re-project our vector data when importing
D) To ensure all our vector and raster data is in the same projection, the feature dataset will automatically re-project our vector and raster data when importing

<!-- C -->


## Downloading Census Data

We want to to download Dissemination Area level population data for the Port Alberni using [Simply Analytics](https://resources.library.ubc.ca/page.php?id=1044).  We are going to download three population variables.  The video below can help guide you through the download process.

* Total Population
* Total Population 60 Years Or Over
* Total Children Living In Households (Children At Home)


<div style="overflow: hidden;
  padding-top: 56.25%;
  position: relative">
  <iframe src="content/images/Distribution.png" title="Processes" scrolling="no" frameborder="0"
    style="border: 0;
   height: 100%;
   left: 0;
   position: absolute;
   top: 0;
   width: 100%;">
   <p>Your browser does not support iframes.</p>
 </iframe>
</div>
<a href="content/images/Distribution.png" target="_blank">View in New Tab</a>

## Downloading Roads Data from DataBC

To conduct the analysis, we’ll also need a roads layer.  This data set is available for download from [DataBC](https://www.data.gov.bc.ca/).  Follow the video instructions to inspect the metadata and request a download. 

**1)** Follow the link and download the roads layer.
* In the Search bar, type “Roads”.
    * Select “Digital Road Atlas (DRA) - Master Partially-Attributed Roads”
	* Whenever downloading data, it is crucial to check the metadata
    * Check your email for the download link (this may take a few minutes).
**2)** Download the data and add it to your PA_Data folder in your PA_RiskAssesment project.
* The layer name isn't very descriptive.  Name it PA_Roads

<iframe width="560" height="315" src="https://www.youtube.com/embed/5jaULGb5ux4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

**3)** Extract the .zip files from DataBC and import them into your PA_Risk_Assessment feature dataset
* The file names from DataBC aren't very descriptive, it might be helpful to change rename them "Roads" and "Coastline".

<img src="Roads.png" alt="hi" class="inline"/>
