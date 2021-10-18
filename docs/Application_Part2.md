---
layout: default
title: Data Classification
parent: Application
nav_order: 2
---


1. TOC
{:toc}



# Defining Rural & Urban Areas

Until 2010, Statistics Canada used a Rural/Urban classification scheme to describe Census unit smaller than a Province/Territory:

**Rural**: a population density less than 400 people per square kilometer **or** a total population of less than 1,000 people.

**Urban**: a unit with a population density at least 400 people per square kilometer **and** a total population of at least 1,000 people.


## How to Applying a Classification Scheme

In this video I show you how to apply the old Urban/Rural Classification to the census subdivisions in BC.  You **do not** need to apply this classification scheme, **but** this video serves as a guide to show you how to apply thee classification scheme we will be using.

<iframe width="560" height="315" src="https://www.youtube.com/embed/uMLtpB6Xjqc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### QA

The Select by Attribute tool lets us use SQL (Structured Query Language) to define expressions for querying vector data. [T/F]


# A Revised Classification

The revised classification method is known as the [Population Centre and Rural Area Classification](https://www.statcan.gc.ca/eng/subjects/standard/pcrac/2016/introduction) and it has four classes:

**Rural**: a population density less than 400 people per square kilometer **or** a total population of less than 1,000 people.
**Small population centers**: not rural **and** a population of between 1,000 and 29,999
**Medium population centers**: not rural **and** a population of between 30,000 and 99,999
**Large urban population centers**: not rural **and** a population of 100,000 and over.


## Applying the Revised Classification

Apply the new Population Centre and Rural Area Classification to the census subdivisions on your own.  The list above hints at how to format your SQL statements.

### WA

Skim the Introduction linked Stats Canada resource page.  What was the reasoning behind updating the classification method?