---
layout: default
title: Geospatial Analysis
parent: Application
nav_order: 3
---

# Geospatial Analysis
{: .no_toc }

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>


# Automating with Model Builder

We’re going to use a tool called Model Builder to organize and save all of our analysis steps in one place.  When we use model builder, if any of our inputs or parameters change, a model can be easily adjusted and rerun at any time.  It also allows us to visualize our analysis process.  This is useful both for editing our own work and sharing it with others.  For a more detailed explanation of Model Builder, check out [this link](https://pro.arcgis.com/en/pro-app/latest/help/analysis/geoprocessing/modelbuilder/modelbuilder-quick-tour.htm).

### QA
Why are we using model builder for this analysis?

<!-- 1) Repeatable 2) changeable 3) Visualize process 4) share workflow -->


# Identify the Inundation Zone

Our criteria for land areas at risk for flooding are: land at or below 10 m elevation and within 1km of the coastline.  I have crated a model to do this part for you (see video below).  In order to identify the land areas in Port Alberni at risk for inundation, we need to do four tasks:

**1**{: .label .label-red } Reclassify the PA_DEM to identify all the areas under 10m elevation. See this link for info on the [Reclassify tool](https://pro.arcgis.com/en/pro-app/latest/tool-reference/spatial-analyst/reclassify.htm).

**2**{: .label .label-red } Convert the reclassified DEM to a polygon. See this link for info on the [Raster to Polygon Tool](https://pro.arcgis.com/en/pro-app/latest/tool-reference/conversion/raster-to-polygon.htm).

**3**{: .label .label-red } Buffer the waterbodies by 1km. See this link for info on the [buffer tool](https://pro.arcgis.com/en/pro-app/latest/tool-reference/analysis/buffer.htm)

**4**{: .label .label-red } Clip the coastline buffer with the inundation zone. See this link for an explanation of the [Clip tool](https://pro.arcgis.com/en/pro-app/latest/tool-reference/analysis/clip.htm).

## Using a Model

I have set up a model to handle the above tasks for you.  Watch the video below for an overview of the model.  Then open/edit the model yourself. To do this, right click the InundationZone model and click "Edit".   Then change the break values in the Reclassify to from 5 to 10 and run the model.  

<iframe width="560" height="315" src="https://www.youtube.com/embed/evyXxnqUKbg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### QA

What is the shape area of the Inundation_Zone?

# Create Your Own Model

We need to figure out:

**1**{: .label .label-red } Which roads are at risk of flooding or damage?
**2**{: .label .label-red } Which properties in the city are at risk?
**3**{: .label .label-red } How many people within Port Alberni and the surrounding area are potentially living in areas at risk?
**4**{: .label .label-red } Are the Tsunami Shelters sufficient?

## Clip the Roads Layer

To answer **1**{: .label .label-red } all we need to do is clip the roads by the inundation zone.  Follow the video below to create a new model and clip the roads layer.  Name the output PA_Roads_Flood.

<iframe width="560" height="315" src="https://www.youtube.com/embed/F_AslIjacNI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Select Properties by Location

To answer **2**{: .label .labe-red} we can use select by location.  See the video below for an explanation of the select by location and instructions on how to apply it in your model.  Name the result Properties_at_Risk.

<iframe width="560" height="315" src="https://www.youtube.com/embed/vqHmErK5J-g" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>




## Question 7)
What is your estimate for the maximum population at risk?  The Population column is listed as Value0 in the attribute table.  *Hint:* Look at the statistics for the column to quickly calculate the sum.  **Note** because of the complexity of this lab, for the numeric answers, I will determine a margin of error based on everyone's answers and give partial credit.  For now the margins have been set to zero, but that will change when we mark the lab.

<!-- 8,820 -->

## Question 8)
Why is the result intersecting the Population_DA_Clip within InundationZone most likely an over esitimate?  Hint: Think about what’s going on with the intersect.  Compare the input with the resulting Population_at_Risk layer. 

<!-- Because were counting all ppl in any DA that even just a has a sliver in the inundation zone -->

## Question 9)
What is the difference between the clip tool and the intersect tool?  You can refer to the lecture video on [vector overlay analysis](https://www.youtube.com/watch?v=jkjVX97Xtcc) and compare the outputs from your intersect (InundationZone) with the outputs from the clips (eg. Population_at_Risk).  *Hint* Look at the attribute tables of the input and output layers.

<!-- Clip is like cookie cutter (just cuts away areas), intersect keeps where two layers overlap &&& combines attributes  -->

## Buffer the Tsunami Warning Sirens and Erase with At Risk Properties

We need to buffer the Sirens layer by 1000m and erase that buffer from the Properties_at_Risk to see if there are any properties that are not adequately served by the tsunami warning sirens.  See the docs for the [erase tool](https://pro.arcgis.com/en/pro-app/latest/tool-reference/analysis/erase.htm)

<iframe width="560" height="315" src="https://www.youtube.com/embed/af2Re9qoVCg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Select the Residential Properties at Risk

Use the ZoningCode.csv file you were given to label identify the zone code for residential and multi-family residential.  Search for Select by Attribute in the geoprocessing pane and to your model, to identify the residential properties at risk.  *Hint* Make sure to select for both residential types (Multi family/Single family) using the OR operator.

<img src="Selection.png" alt="hi" class="inline"/>

## Question 10)
Why are we using the OR operator if we want both multi AND single family residential properties?

<!-- and is only for selecting for conditions between columns, because a property can only have one zone value.  it can be single and multi family  Or can be used within.   -->

## Question 11)
How many residential properties are at risk of Inundation?

<!-- 690 -->
