- [ ] Use binomial distribution
	- Number of years with positive migration per decade
- [ ] Use poisson distribution 
	- Number of people in each age bracket
- [x] Use linear regression ✅ 2023-11-01
	- Population at future dates using lags of other variables
	- Compare lasso, ridge, elasticnet 
	- Compare RF-Regressor
	- Compare to ARIMA
	- Try SVM regressor
	- Refer to CRISP-DM
 
 Investigate best model selection using gridsearch.cv_results_ - might be ties
 Regressor.score gives R^2 - extract for RF
 Try polynomial features - interaction between population/migration/emigration?
 Graph of test R^2 comparison
 
- [ ] Add annotations / justfication to machine learning section
	- Reformat confusion matrices and discuss results

- [ ] Import and clean town data
	- Probably could get away with two data points - allows for growth feature and demonstrating cleaning
	 - Extract county / townland feature from names -  demonstrates relatively involved data cleaning 
	  - Look at sizes of towns - are they lognormal? Can we extract a town_size variable?
   
- [ ] Use KNN 
	- Group towns together
	- Compare with naive bayes
- [ ] Find references 
	- [ ] Discrete distributions 
		-  Jaynes?
		- Weiss - Introductory Statistics
	- [ ] ML techniques 
		- 100 page machine learning book 
		- Elements of Statistical Learning
		- Introduction to Statistical Learning
	- [ ] CRISP-DM
	- [ ] Programming techniques / style
		- PEP-8- python enhancement proposal
		- Clean Code
- [ ] Reread Assignment Brief & make sure everything is covered
- [ ] Write Word Doc report
	- What's my angle? - An Investigation into Irish Emigration trends in the 21st Century 