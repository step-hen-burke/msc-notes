---
title: Data Preparation for Duplicate Detection
authors: Ioannis Koumarelas, Lan Jiang, Felix Naumann
year: 2020
---

The authors outline a way to chain many candidate data transforms together, then iteratively remove them where there's no change or an improvement in AUC-PR - minimizing the set of transformations.

They're mostly focused on duplicate detection, but the problems they describe about ad-hoc data treatment apply more broadly.

In their datasets, doing all transformations carelessly sometimes gave worse results than doing nothing. 

_This could possibly be used in conjunction with an orchestration framework like Airflow to prune an execution DAG prior to deployment. Or more simply, editing a sklearn pipeline_

![](drawings/@koumarelasDataPreparationDuplicate2020%202023-09-22%2010.31.26.excalidraw.png)
%%[🖋 Edit in Excalidraw](@koumarelasDataPreparationDuplicate2020%202023-09-22%2010.31.26.excalidraw.md), and the [dark exported image](@koumarelasDataPreparationDuplicate2020%202023-09-22%2010.31.26.excalidraw.dark.png)%%