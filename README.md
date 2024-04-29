# codecademy-weight-ml
This project was a quick review of machine learning, logistic regression, and a comparison of feature selection through various wrapper methods.

It was done using scikit learn, in a Jupyter Notebook framework that was provided by Codecademy.com, with Py 3.10.12. The libraries and methods used include:
* pandas
* sklearn
    * .linear_model - LogisticRegression
    * .preprocessing - StandardScaler
    * .feature_selection - RFE
* mlxtend
    * .feature_selection - SequentialFeatureSelector
    * .plotting - plot_sequential_feature_selection
* matplotlib.pyplot

The dataset  was provided by Codecademy, using data from from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Estimation+of+obesity+levels+based+on+eating+habits+and+physical+condition+). Categorical variables were changed by Codecademy to numerical ones in order to facilitate analysis. The dataset includes 2111 survey response on lifestyle and weight, with 18 total features and one binary outcome variable indicating obesity. 

In this dataset, there were 18 possible predictor variables. The methods applied and evaluated were:
* Logistic Regression, lr, of all 18 predictor features
* Sequential Forward Selection, sfs,  with Logistic Regression with a max feature selection of k=9
* Sequential Backward Selection, sbs, with Logistic Regression with a max feature selection of k=7
* and, Recursive Feature Elimination, rfe,  with Logistic Regression and a max feature selection of n=8.

The respective accuracy of the models were as follows:
* Logistic Regression, 18 features: 76.6%
* Sequential Forward Selection, 9 features: 78.3%
* Sequential Backward Selection, 7 features: 76.4%
* Recursive Feature Elimination, 8 features: 76.8%

