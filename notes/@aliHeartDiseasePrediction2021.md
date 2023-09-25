---
title: "Heart disease prediction using supervised machine learning algorithms: Performance analysis and comparison"
authors: "Md Mamun Ali, Bikash Kumar Paul, Kawsar Ahmed, Francis M. Bui, Julian M.W. Quinn, Mohammad Ali Moni"
year: 2021
---

Keywords: #MachineLearning #SupervisedLearning #KNN #DecisionTrees

The authors use supervised machine learning techniques to predict the presence of heart disease within a kaggle dataset.

I have some concerns about some of their data cleaning steps. Their outlier removal was a bit naiive, they just cut off anything outside of the IQR, and then got 100% accuracy. I don't think removing those data points was necessarily justified. 

100% accuracy with KNN and a single decision tree feels suspicious anyway, particularly in health sciences.