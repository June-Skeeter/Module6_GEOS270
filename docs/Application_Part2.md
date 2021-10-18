---
layout: default
title: Data Classification
parent: Application
nav_order: 2
---

# Data Classification
{: .no_toc }


1. TOC
{:toc}

# Defining Rural & Urban Areas

Until 2010, Statistics Canada used a Rural/Urban classification scheme to describe Census unit smaller than a Province/Territory:

**Rural**: a population density less than 400 people per square kilometer **or** a total population of less than 1,000 people.

**Urban**: a unit with a population density at least 400 people per square kilometer **and** a total population of at least 1,000 people.

---

## A Revised Classification

Statistics Canada Now uses the Population Centre and Rural Area Classification:

|**Rural**         |**Small population centers**            |**Medium population centers**                                            |**Large urban population centers**        |
|------------------|----------------------------------------|-------------------------------------------------------------------------|------------------------------------------|
|Same as old method|Not Rural **and**<br>Population < 30,000|Not Rural **and**<br>Population >= 30,000 **and**<br>Population < 100,000|Not Rural **and**<br>Population >= 100,000|

### WA

Skim the Introduction of the [Documentation](https://www.statcan.gc.ca/eng/subjects/standard/pcrac/2016/introduction) explaining the classification scheme.  What was the reasoning behind updating from the old Rural/Urban method?

---

# How to Apply the Classification

In this video I show you how to apply the old Urban/Rural Classification to the census subdivisions in BC.  You **do not** need to apply this classification scheme. This video serves as a guide, after watching it, apply the Population Centre and Rural Area Classification to the census subdivisions on your own.  The table above hints at how to format your SQL statements.

<iframe width="560" height="315" src="https://www.youtube.com/embed/uMLtpB6Xjqc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### QA

The Select by Attribute tool lets us use SQL (Structured Query Language) to define expressions for querying vector data. [T/F]

