# Predicting-Algerian-Forest-Fires-with-Machine-Learning
Predicting Algerian Forest Fires with Machine Learning

Introduction-

Starting in June 2012, the Bejaia and Sidi-Bel Abbes regions of Algeria experienced numerous wildfires that likely resulted from a heat wave. The fires burned throuh Algeria’s pine and cork oak forests, damaging a total area of 295 square kilometers.

Purpose of Analysis-

Do weather metrics in the Algerian regions determine the occureces of forest fires? How distinct are weather metrics for forest fires? How can we detect fires before they occur?

We uses machine learning to process features and predict whether or not a fire will occur based on significant attributes. Our model is based on data from Bejaia and Sidi-Bel Abbes, but we aim to build more robust and generalizable models that can help policy makers in different regions implement precautionary measures against fires before they strike.

Assumptions-

In our analysis, we assume that the response variable is binary. The response variable is the class ‘fire’ or ‘not fire.’ We do not consider midway situations, such as fires that were close to ignition but utimately faded. We assume that our observations are unique instances with no extreme outliers. We also deduce that the samples are representative and large enough to make justifiable predictions.


Data Cleaning-

The data is originally formatted as two stacked datasets where the top corresponds to Bejaia and the bottom correponds to Sidi-Bel Abbes. We combine them into one dataframe and create a ‘Region’ variable to distinguish regions. We reset the index and polish the column names for easy manipulation.

Exploratory Data Analysis-

We first examine the correlation between all pairs of attributes except ‘date’ and ‘time’. We find that some variables are highly correlated with one another, such as BUI and DC. These findings are later reflected in our feature selection process in modeling to avoid multicollinearity.

Machine Learning Algorithms-

The following machine learning algorithms have been implemented on the data:

Linear Regression Model
Lasso Regression
Ridge Regression
ElasticNet Regression

The results of the machine learning models are compared and evaluated, and the best performing model is selected based on its accuracy.
