---
title: Use Case and Performance Analyses for Missing Data Imputation Methods in Big Data Analytics
authors: Lan Yang, Jason Amaro Chiang
year: 2020
---

Keywords: #Imputation #MissingData #DataCleaning #EDA 

Carried out on time series data - linear interpolation and last seen imputation work well, possibly because missings and actual values in time series are often autocorrelated, but they insert missings randomly. I think the downfalls of last seen in particular would be more apparent in a real time series with missings that are clumped together.

The title says big data analytics but their datasets only have 21 and 1259 rows.

Missing data types:
>(1) Missing Completely at Random (MCAR) There is no relationship between the missingness of the data and any values observed or missing. There is nothing systematic going on that makes some data more likely to be missing than others. All data points share the same probability of going missing. Common examples are forgetting to fill an entry in a survey, dropping a test tube and omitting the data collected on it. 
>
>(2) Missing at Random (MAR) In this category, there is a systematic relationship between the propensity of missing values and the observed data but not the missing data itself. For example, members of a library who live farther to that library are possibly to have more overdue books. 
>
>(3) Missing Not at Random (MNAR) There is a relationship between the propensity of a value to be missing and its hypothetical value. For example, people with high salaries are less likely to report income in a survey, people who have many overdue books are less likely to report how many overdue books they have because it is embarrassing.
