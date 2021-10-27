---
layout: default
title: Spatial Analysis
parent: Content
has_children: True
nav_order: 1
---

# Spatial Analysis Methods
{: .no_toc }

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

Spatial analysis methods are central to the effective application of GIS.

# Vector Methods

## Overlay

- [Clip](https://pro.arcgis.com/en/pro-app/latest/tool-reference/analysis/clip.htm)
- [Intersect](https://desktop.arcgis.com/en/arcmap/latest/tools/analysis-toolbox/intersect.htm)
- [Identity](https://desktop.arcgis.com/en/arcmap/latest/tools/analysis-toolbox/identity.htm)
- [Union](https://desktop.arcgis.com/en/arcmap/10.3/tools/analysis-toolbox/union.htm)
- [Erase](https://desktop.arcgis.com/en/arcmap/10.3/tools/analysis-toolbox/erase.htm)
- [Symmetric Difference](https://desktop.arcgis.com/en/arcmap/10.3/tools/analysis-toolbox/symmetrical-difference.htm)
- [Spatial Join](https://pro.arcgis.com/en/pro-app/latest/tool-reference/analysis/spatial-join.htm)
	- Combine attributes, without 

## Proximity Analysis

- Buffer:
	- [Single Buffer](https://pro.arcgis.com/en/pro-app/latest/tool-reference/analysis/buffer.htm)
		- Create polygon around a point, line, or polygon feature.
		- Single set distance, or specified by field

	- [Multi-Ring Buffer](https://pro.arcgis.com/en/pro-app/latest/tool-reference/analysis/multiple-ring-buffer.htm)
		- Useful for multi-criteria buffers

- [Select by Location](https://desktop.arcgis.com/en/arcmap/10.3/map/working-with-layers/using-select-by-location.htm)
	- Containment
		- Point in Polygon
		- Lines or Polygons that overlap a feature
	- Intersection
		- Containment + Any line/polygon that touches a feature - does not require full containment

## Aggregation

- [Dissolve](https://pro.arcgis.com/en/pro-app/latest/tool-reference/data-management/dissolve.htm)


# Raster Methods

## Overlay

- Zonal
	- [Zonal Statistics](https://desktop.arcgis.com/en/arcmap/10.3/tools/spatial-analyst-toolbox/zonal-statistics.htm)
	- [Zonal Statistics as Table](https://pro.arcgis.com/en/pro-app/latest/tool-reference/spatial-analyst/zonal-statistics-as-table.htm)

- [Weighted Overlay](https://desktop.arcgis.com/en/arcmap/10.3/tools/spatial-analyst-toolbox/weighted-overlay.htm)
	- Combine multiple layers for suitability or risk analysis
	- Suitable alternative for the Port Alberni Tsunami Modelling

- [Raster Calculator](https://desktop.arcgis.com/en/arcmap/10.3/tools/spatial-analyst-toolbox/raster-calculator.htm)
	- More general than weighted overlay, can be used to do weighted overlay if combined with reclassification.
	- Suitable alternative for the Port Alberni Tsunami Modelling

- [Clip](https://pro.arcgis.com/en/pro-app/latest/tool-reference/data-management/clip.htm)
	- Cuts raster down to a bounding box.  Bounding box extent can be defined by another raster layer, a vector layer, or manually.

## Surface Analysis

- [Slope](https://desktop.arcgis.com/en/arcmap/10.3/tools/spatial-analyst-toolbox/slope.htm)
- [Aspect](https://pro.arcgis.com/en/pro-app/latest/help/analysis/raster-functions/aspect-function.htm)

## Aggregation

- [Reclassify](https://pro.arcgis.com/en/pro-app/latest/tool-reference/spatial-analyst/reclassify.htm)

