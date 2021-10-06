---
layout: default
title: Choosing a Data Model
parent: Phenomena and Data Types
grand_parent: Content
# has_children: True
nav_order: 4
---

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

## Choice of Data Model
Vector data has some important advantages:

  The geometry itself contains information about what the dataset creator thought was important
  The geometry structures hold information in themselves - why choose point over polygon, for instance?
  Each geometry feature can carry multiple attributes instead of just one, e.g. a database of cities can have attributes for name, country, population, etc
  Data storage can be very efficient compared to rasters

The downsides of vector data include:

  potential loss of detail compared to raster
  potential bias in datasets - what didn’t get recorded?
  Calculations involving multiple vector layers need to do math on the geometry as well as the attributes, so can be slow compared to raster math.

Vector datasets are in use in many industries besides geospatial fields. For instance, computer graphics are largely vector-based, although the data structures in use tend to join points using arcs and complex curves rather than straight lines. Computer-aided design (CAD) is also vector- based. The difference is that geospatial datasets are accompanied by information tying their features to real-world locations.
