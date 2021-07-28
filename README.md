# SEABuildingEnergyBenchmarking
11 Regression Models Comparision


The mains steps in the notebook1 :
  -Data Preparation to merge the 2015 and 2016 datasets
  -Data Processing in some columns values
  -Rows Selection
  -Duplicates on OSEBuildingID column
  -Redundant columns
  -Features Selection
  -Feature Engineering : new columns
  -Outliers Analysis
  -Exploratory Data Analysis
  -Correlation Matrix to avoid correlation between variables
  -Correlation Analysis between X and y
  -Correlation ANalysis between categorical and numerical variables
  -Final Features Selection
  -NaN imputer methods comparison 
  -NaN KNN Imputer

The mains steps in the notebook2 :
  -Data Preparation on rows and columns
  -Normalisation on numerical X
  -Dummies for categorical X
  -Log transformation for y1 and y2
  -Cross Validation on train to select the best model without ENERGYSTARScore : GBR - Gradient Boosting Regressor.
  -Train and Performance Measures on train and test sets to select the bes model : AdaBoost 
  -Scatter plot between y_test and y_pred for all models
  -Importance variable with the best model selected AdaBoost
  -GridSearch for Hyperparameters on AdaBoost without and with ENERGYSTARScore to compare

Finally, the best model is : 
  -AdaBoost without ENERGYSTARScore and without GridSearch for y = GHGEmissions(MetricTonsCO2e)
  -AdaBoost without ENERGYSTARScore for y = SiteEnergyUse(kBtu)
