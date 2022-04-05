---
layout: default
title: Exam Review
parent: Lecture Content
has_children: True
nav_order: 5
---

# Final Exam Review

## Essays (x3)

* No definitive word count/limit.  Responses can be brief, but should be thorough - answer all parts of the question.

* You can expect:
  * 1 essay on spatial coordinate systems (Module 1)
    * Randomly assigned from bank
  * 1 essay on spatial data models (Module 2)
    * Randomly assigned from bank
  * 1 essay on other topics from the course
    * Given a choice from multiple prompts.  Possible topics (principals of map design, uncertainty, ethics)

## Flowchart (x1)

* Tests your ability to work through a problem using GIS methods.  Create a flow chart outlining a GIS analysis in response to a prompt.

### Flowchart Practice Question

**Prompt**: Based on your analysis from the Tsunami Risk Assessment, the city of Port Alberni has been given funding build a new evacuation shelter.  You have been tasked with finding a suitable location for the shelter.

**Criteria**: The shelter must

* Be located outside of any potential inundation zone (Elevation > 15 m **or** distance from coastline > 1 km).
* Be at least 1 km away from existing shelters.
* Service at least 1,000 residents (assume 1 km radius for service area)
* Located no more than 250 m away from an Arterial Roadway

**Data**

|Name      |      Type          |  Coordinate System  |  Attributes |
|----------|--------------------|---------------------|-------------|
|Digital Elevation Model |Raster|UTM Zone 10N | Elevation (m) |
|BC Coastal Boundary File|Vector (line) |UTM Zone 10N | Name |
|BC Roads Layer |Vector (line) |UTM Zone 10N | Road Type (Arterial/Residential/Private), Name |
|Census Dissemination Areas |Vector (polygon) |UTM Zone 10N | Population, Income, Housing Cost |
|Current Shelters |Text (.csv)|WGS 1984 | Latitude/Longitude, Name, Capacity |


### Short Answer

Generally, 1-3 sentences will suffice.  Try not to write much more than a paragraph.  Bullet point lists are sufficient where applicable.

### Miscellaneous Questions

Mix of matching, fill in the blank, multiple choice, etc. (~ 15%)

