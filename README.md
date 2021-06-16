# Boston-Housing-Price-Prediction
# Introduction

This is a basic Machine Learning Project dealing in Predicting Housing Prices in the city of Boston, the capital of Massachusetts in the United States. The dataset (Boston Housing Price) was taken from the StatLib library which is maintained at Carnegie Mellon University and is freely available for download from the UCI Machine Learning Repository or we can load it directly from scikit-learn Library. The dataset consists of 506 observations of 14 attributes(features). The median value of house price in $10000s, denoted by MEDV, is the outcome or the dependent variable in our model. Below is a brief description of each feature and the outcome in our dataset: Variables:

* 1.CRIM – per capita crime rate by town
* 2.ZN – proportion of residential land zoned for lots over 25,000 sq.ft
* 3.CHAS – Charles River dummy variable (1 if tract bounds river; else 0) 
* 4.NOX – nitric oxides concentration (parts per 10 million)
* 5.RM – average number of rooms per dwelling
* 6.AGE – proportion of owner-occupied units built prior to 1940
* 7.DIS – weighted distances to five BostLSTAT - % lower status of the population on employment centres
* 8.RAD – index of accessibility to radial highways
* 9.INDUS – proportion of non-retail business acres per town
* 10.TAX – full-value property-tax rate per $10,000
* 11.PTRATIO – pupil-teacher ratio by town
* 12.B – 1000(Bk - 0.63)^2 where Bk is the proportion of blacks by town 13. LSTAT – % lower status of the population
* 13.LSTAT - % lower status of the population 
* 14.MEDV – Median value of owner-occupied homes in $10000’s

# Softwares and Libraries

This Projects uses the following softwares and libraries:
* Jupyter Notebook
* Python
* numpy
* pandas
* matplotlib
* seaborn
* scikit-learn

# Machine Learning Models used

* In this project i have implemented a Basic Linear Regression Model from scratch with gradient descent as an optimization technique and RSquared(r2score)  and Root Mean Squared(RMSE) error as evaluation metrics.
* LinearRegression Model from scikit-learn library.
* DecisionTree Regression Model from scikit-learn library.
* Random Forest Regression Model from scikit-learn library.

# Description

The Aim is to analyze the data(Boston Housing) ,build a model that best performs on the data and to predict value of a house given its features,
Here I have loaded the data from scikit-learn library ,transformed the data into the DataFrame containing 14 attributes including 'MEDV',the target variable(Dependent Vaariable).
Next, I have performed Exploratory Data Analysis using seaborn(regression plot, box plot, heatmap, distplot) and matplotlib(subplots).
You can find the observations of analysis in the .ipynb notebook here in the repository.
Then, I have divided the data into train and test set using sklearn's train_test_split.
Next, I trained my linear_regression model implemented from scratch -performed gradient descent , then i evaluated the models performance on the test set using Mean Squared Error, Root Mean Squared error and Rsquared evaluation metrics.
Then i went on and trained Decision Tree and Random Forest models on train set and evaluated respective model performances on test set.
Next, I performed GridSearch with KFold CrossValidation taking RandomForest  model on Entires dataset, later on on basis of analysis of data obatined in Data Analysis step.
I have removed some of the outliers and features and trained the RandomForest model on resulatant data.
Finally, after all the data exploartion and training various models RandomForest Model with n_estimators=100 gave me the best performance.
-For complete Details go through .ipynb notebook.


