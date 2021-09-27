---
layout: default
title: Assessment
nav_order: 4
---

# Assessment
{: .no_toc }

You can use the course Canvas page to complete the quiz, written submission, and files uploads.  I suggest you download write down your answers as you progress through the Content and Application sections then upload your answers to canvas once you have finished the module.

1. TOC
{:toc}

---

# Module Quiz

All quiz answers are multiple choice, numeric input, fill in the blank, etc. type questions.  They can be submitted via the Module 1 Quiz that can be found on the Canvas page.  You will have unlimited attempts to take the quiz.

## Application Questions

[**QA1**](Application_Part3.md#qa1)
For every $100 increase in income at the CT level, how much does rental price increase?

[**QA2**](Application_Part3.md#qa2)
What is the r2 score for this model?

[**QA3**](Application_Part3.md#qa3)
Which Census Unit displays a more direct relationship between income and housing?
- DA
- CT
- About the same

[**Q4**](Application_Part3.md#qa3)
Which value denotes the lower bound of the "Green Vegetation Class?"

[**Q5**](Application_Part4.md#qa5)
What is the DAUID of the DA with the highest Mean NDVI value?  *Hint* Double clicking on Green Veg Area in the attribute table allows you to sort in ascending/descending order.

[**Q6**](Application_Part4.md#qa6)
What is the DAUID of the DA with the highest Green Veg Area?

[**QA7**](Application_Part4.md#qa7)
Is the DA with the highest mean NDVI value the same as the DA with the greatest area of green vegetation? Y/N

[**QA8**](Application_Part4.md#qa8)
Create a scatter plot, with the Mean NDVI value (Output from Method 1) on the X-axis and Green Veg Area Sum (Output from Method 2) on the Y-axis.  What is the R2 value? 

[**QA9**](Application_Part4.md#qa9)
The r2 score indicates Mean NDVI value is [Strong/Moderate/Weak/Very Weak] predictor of Green Veg Area.

[**QA10**](Application_Part4.md#qa10)
Change the Y-axis to Income and leave the X-axis as Mean NDVI, note the R2 score.  Now change the X-axis to the Green Veg Area Sum and note the R2 score.  Which variable has a "stronger" relationship with income? [Green Veg Area/Mean NDVI]

[**QA11**](Application_Part4.md#qa11)
Are either of these variables strongly linked to income? [Yes/No/Just Mean NDIV/Just Green Veg Area]

[**QA12**](Application_Part5.md#qa12)
Create a scatter plot, with the Mean NDVI value (Output from Method 1) on the X-axis and Green Vegetation Fraction (Normalized Output from Method 2) on the Y-axis.  What is the R2 value? 

[**QA13**](Application_Part5.md#qa13)
The r2 score indicates Mean NDVI value is [Strong/Moderate/Weak/Very Weak] predictor of Green Veg Area.


---

## Content Questions

[**QC1**](Content_Part1.md#qc1)
The ______ data model represents space as a continuous grid of ______ which each contain a single ______.

[**QC2**](Content_Part1.md#qc2)
The ______ data model represents features in space as discrete two-dimensional ______ , one-dimensional ______ , and/or "zero-dimensional"  points.  Attribute information is stored separately in a ______.

---

# Module Assignment

All written answers should be numbered and record in one document, saved as a .pdf, and uploaded to canvas.  The file submissions should also be saved as .pdf and uploaded as a separate document.  **Written answers can be as brief as you want as long as they answer the question.**

## Application Questions

### Written Answers

[**WA1**](Application_Part2.md#wa1)
What is NDVI and what is it used for?  Describe the patterns you see in NDVI across the metro Vancouver area.

<!-- NDVI is a metric for gauging vegetation health/density/"greenness".  It is based off the differential reflectivity between red (low for plants) and near infrared (high for plants).  Across metro van - water/concrete low, residential w/ tree cover medium, forests/agriculture high -->

[**WA2**](Application_Part3.md#wa3)
What are the differences you notice between the CTs and DAs in terms of size and population?

<!-- CDAs are smaller population/size wise, DAs give full coverage CTs only in CMA (metro areas) -->

[**WA3**](Application_Part5.md#wa3)
What does data normalization do? How does normalizing effect the relationship with income? Create a new chart with Green Vegetation Fraction on the X-axis and Income on the Y-axis to find out.  How does this compare to when we were looking at the relationship between Total Green Vegetation Area and income?

<!-- Normalizing accounts for a confounding/secondary/other variable by dividing the variable of interest by the confounder.  This helps control for correlation between the two variables. The R2 score goes up to 0.083, Accounting for the different sizes of the DA "improves" the relationship. But not by much -->

[**WA4**](Application_Part6.md#wa4)
What do the results of this analysis show?  Are there any improvement you think we could make to this analysis?

<!-- The relationship isn't strong, probably because there are other factors that are determine where people with limited resources can afford to live and where those with money choose to live. (7.5 pts)

Things to look at might include: housing cost (rent or land value) instead of income.  Both NDVI & green area combined (eg. multivariate linear regression). Excluding downtown core and focus on just medium density residential areas.  Account for water/beaches (also attracts high income but low NDIV)  .  These are just possible suggestions, they don't have to list these anything that makes sense counts (7.5 pts for listing two or more suggestions, 3.25 pts if just one). -->


### File Submissions

[**FA1**](Application_Part6.md#fa1)
Export your Layout as a .pdf and upload it to Canvas.

<!-- See example map:

Map showing proper mean NDVI (not green fraction) - 5pts

Chart showing proper mean green fraction vs income (not NDVI) - 5pts

Source statement (Name/source/data/date) - 4ts (1 off for name/date etc.)

Clean presentation & appropriate elements (Text is descriptive/not cut off, north arrow, legend, scale text) - 6 pts

Projection and scale 1:100,000 (should be obvious if the left it in Lambert conformal, Vancouver will be slanted)  - 5pts
 -->

---

## Content Questions


---

# Rubric 

All written answers and file submissions will be scored using this generic rubric.  Your TA will provide brief comments where applicable.  For more feedback you can follow up with your TA.

|Score|Comments            |
|-----|--------------------|
| 0%  |Missing             |
| 25% |Insufficient        |
| 50% |Below Expectations  |
| 75% |Met Expectations    |
| 100%|Exceeds Expectations|
