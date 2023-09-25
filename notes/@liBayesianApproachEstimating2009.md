---
title: "A Bayesian Approach for Estimating and Replacing Missing Categorical Data"
authors: "Xiaobai Li"
year: 2009
---

Keywords: #Bayesian #CategoricalData #DataCleaning #Imputation #MissingData #EDA

The authors use [[Bayes|Bayesian]] methods to impute missing data.

Only works on categorical data - numeric data must use other methods or coerce the 
variable to a category - e.g. with range splits

Assumes variables are independent to ease calculation. 

Calculates the probability of each class given the marginal occurrence of the classes in the nonmissing data.

Two imputation methods:
- Assign missings to the class with the highest marginal probability (MaxPost: Maximum posterior probability)
- Randomly draw from a distribution following the marginal probabilities (PropPost: Proportional posterior probability)

MaxPost overweights the max class when the data is missing randomly, but this disadvantage can disappear when the data is nonrandomly missing, as is often the case.
