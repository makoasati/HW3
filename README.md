# Week 3, Spring 2026

For this week's homework:
1. Read the ipynb in this repo that shows you how to convert columns with special characters such as commas and dollar signs. There's nothing to turn in related to this notebook.
2. Read the ipynb in this repo that includes more groupby and transform examples. This file is an extension to the groupby's shown in the cereal example.
3. **Turn in an EDA on one of the following datasets.** I strongly encourage you to do this analysis on your own, asking ChatGPT for help only with syntax (e.g. "How do I do a groupby on two variables and calculate the means for each in Python using Pandas"). You could easily just give ChatGPT the URL to the dataset and ask for a completed EDA, but you're going to learn very little that way. 

**Datasets are ordered from easiest to most difficult, choose your own adventure.** I've given hints about the data cleaning you may have to do. They all come from the state of Iowa because they have the best and cleanest open datasets! 


* [Math and Reading Proficiency in Iowa by Year, District, and Grade](https://data.iowa.gov/Primary-Secondary-Ed/Math-And-Reading-Proficiency-in-Iowa-by-School-Yea/f3h8-mnxi/about_data)
  - Numeric columns should import as numeric, should require relatively little cleanup. But there may still be some missing data! 
  - Small dataset, ~70k rows 

* [Iowa Quartery Retail Sales](https://data.iowa.gov/Taxes-Tax-Credits/Iowa-Quarterly-Retail-Sales-Tax-Data-by-12-Busines/wsde-3id9/about_data)
  - Most of the numeric columns will require some cleanup. For example, some rows have "S" in them to indicate that this value was suppressed due to too few observations in a given category. You'll have somehow deal with this before you can convert the rest of the column into numeric.
  - Moderately sized dataset, ~130k rows
 
* [State of Iowa Salary Book](https://data.iowa.gov/Government-Employees/State-of-Iowa-Salary-Book/s3p7-wy6w/about_data)
  - Base salary column will be difficult to clean. You'll have to find all the unique strings in there, remove them, then correctly multiply the base salary column by the time period (e.g. monthly or biweekly pay).
  - Large dataset, ~1M rows
 
# What to include in an EDA

Refer to what we did in week 1 as a reminder of how to conduct an EDA. 
* Include an introduction that sets up the **target audience** of the analysis, including why they should care
* Include a mix of different types of analyses (e.g. info, describe, value counts, groupby, check for missing data)
* Include a brief conclusion stating what you learned from the EDA. If you found errors in the data, include that in the conclusion
  
