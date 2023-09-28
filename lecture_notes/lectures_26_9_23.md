# Machine learning:

Keywords: #MachineLearning #SupervisedLearning #DecisionTrees #GINI #DataNormalization #sklearn #KNN
## Finishing off Tutorial 1

How to choose the optimal value of KNN - is there a formal method? Something like AIC that penalises higher values of K but also takes train & test accuracy into account?
- [x] Find a paper on numerical strategies for choosing optimal values of N in KNN ✅ 2023-09-28
[[@hassanatSolvingProblemParameter2014]]

sklearn.classification_report  definitions - f score, weighted avg, macro avg etc.
- [x] Read documentation on sklearn.classification_report ✅ 2023-09-28
https://scikit-learn.org/stable/modules/generated/sklearn.metrics.classification_report.html
Docs for sklearn.precision_recall_fscore_support gives an explanation of the terms https://scikit-learn.org/stable/modules/generated/sklearn.metrics.precision_recall_fscore_support.html#sklearn.metrics.precision_recall_fscore_support
Macro + micro avg explanation:
https://datascience.stackexchange.com/questions/15989/micro-average-vs-macro-average-performance-in-a-multiclass-classification-settin

Why normalize / standardize data? Why isn't it done with iris?
- [x] Read up on reasons why normalizing data is performed ✅ 2023-09-28
https://towardsai.net/p/data-science/how-when-and-why-should-you-normalize-standardize-rescale-your-data-3f083def38ff
https://developers.google.com/machine-learning/data-prep/transform/normalization

Why was petal width removed in Tutorial 1? Apparently due to analysis of the heatmap but I'm unsure why exactly - we see later that it has low feature importance using RF

## RF & Decision Trees

Review Decision Tree growth algorithm differences - Hunt's, CART, etc.
- [x] Find a paper comparing difference Decision Tree algorithms ✅ 2023-09-28
[[@zharmagambetovExperimentalComparisonOld2019]]

Categorical splitting justification - gini impurity, entropy etc.
- GINI index is an impurity calculation - for each node in a split you get a measure based on the probability of seeing each class in the split nodes. If the weighted gini between child nodes is greater than the parent node's gini, you have positive gain, so a split is justified.

- Entropy is an alternative split criterion 
- [x] What are the differences between GINI and Entropy? ✅ 2023-09-28
https://www.geeksforgeeks.org/gini-impurity-and-entropy-in-decision-tree-ml/
https://datascience.stackexchange.com/questions/10228/when-should-i-use-gini-impurity-as-opposed-to-information-gain-entropy

- Error is not typically used because of linear behaviour - sharp inflection / gradual slope to the maximum gives small differences where the model should be unsure?
- [x] Why is GINI / Entropy preferred to Error? ✅ 2023-09-28
https://stats.stackexchange.com/questions/140858/when-is-classification-error-rate-preferable-when-pruning-decision-trees

Entropy and GINI change in smaller degrees, so in some cases they can split with a small gain where the error gain would be 0, and it'd stop splitting prematurely.
https://sebastianraschka.com/faq/docs/decisiontree-error-vs-entropy.html

_fit_transform() vs transform()_ - fit_transform fits its parameters to the sklearn object, then transforms the input. transform uses an already fitted transformer, so test data should only be transformed by transform, not fit_transform - https://stackoverflow.com/questions/59101623/how-to-use-fit-and-transform-for-training-and-testing-data-with-standardscaler

- [x] How does the decision tree choose its splits / rules - trying many in order to maximise gain? ✅ 2023-09-28
Multiple possiblilities for categorical target - gain, gini, chi-sq
Continuous target -> reduction in variance
https://www.analyticsvidhya.com/blog/2020/06/4-ways-split-decision-tree/

Choosing a continuous split -> sort the values and evaluate the midpoints between values for gain/gini/whatever
https://datascience.stackexchange.com/questions/24339/how-is-a-splitting-point-chosen-for-continuous-variables-in-decision-trees

# Data Visualisation

Keywords: #EDA #Imputation

_Data is fact gathered within a specific context_

Imputation:
- Imputation & removal always needs to be justified. 
- Outliers shouldn't be dropped without justification, they're always useful.
- Business needs and needs of the data problem might be contrary - decisions made from the business PoV can introduce bias
- The business problem is secondary to exploring and understanding the data

#### Discussion on Assignments
- Assignments are primarily evaluated on the justification & intention behind decisions made
- Need to reference in the literature why things are correct and when they've been done before, choice through experimentation may not be sufficient
- Due around week 6/7 - will have about a month to do it - integrated through all 4 modules
- On Saturday classes: David himself doesn't plan on giving us Saturday classes unless there's a good reason for it

- _Focus on capturing the justification for applying EDA techniques when reading_

