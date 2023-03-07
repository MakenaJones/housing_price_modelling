# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 2: Ames Housing Data and Kaggle Challenge 


### Problem Statement

Are certain housing features associated with higher sales prices? Are the main drivers of housing prices structural and difficult to change, or are there certain features a homeowner can hope to change to add to increase the price of a house? 

---

### Datasets

#### Provided Data

The following provided data sets were used in this analysis:

* [`train.csv`](../data/train.csv): 

* [`test.csv`](../data/test.csv): 


#### Data Dictionary

The main dataset has an extensive data dictionary: ([source](https://www.kaggle.com/competitions/dsir-1128-project-2-regression-challenge/data)

Additional variables created during the modelling process are featured below.

|Feature|Type|Dataset|Description|
|---|---|---|---|
|train_clean.csv|data frame| train.csv|Train data without columns not used in model, null values filled and dummy columns added.
|test_clean.csv|data frame| test.csv|Test data without columns not used in model, null values filled and dummy columns added.
|kaggle_model.csv|data frame|test_clean.csv|House sale price predictions for Kaggle.
|lasso_model.csv|data frame|test_clean.csv|House sale price predictions using lasso regularisation.
|ridge_model.csv|data frame|test_clean.csv|House sale price predictions using ridge regularisation.
|not_remodelled|column|train_clean.csv,test_clean.csv|House has not been renovated/remodeled.
|no_pool|column|train_clean.csv,test_clean.csv|House does not have a pool.
|no_fireplace|column|train_clean.csv,test_clean.csv|House does not have a fireplace.

#### Primary Findings and Conclusions

Sale Price Multiple Linear Regression Model Coefficients: 

|Feature|Coefficient|
|---|---|
|Duplex|-18050.060004|
|Townhouse Inside Unit|-15613.695881|
|Townhouse End Unit|-10751.100709|
|No Remodel|-9856.513834
|No Fireplace|-9745.074356|
|2.5 story:2nd Level Unfinished|-9010.192718|
|2 Family Conversion|-2405.863749|
|2 Story|-550.681044|
|House Age|-432.350415|
|Lot Area|0.834023|
|Total Basement Area|12.278061|
|Garage Area|38.976527|
|Above Ground Living Area|51.283077|
|Split Level|3732.275411|
|1 Story|12567.139463|
|1.5Unf|16761.107787|
|Split Foyer|19042.816344|
|Overall Quality|21775.803903|
|2.5 Stories|26262.943041|
|No Pool|76587.810325|

To answer my problem statement, certain features are undoubtably associated with higher prices, but they seem to be structural and hard to necessarily change for a homeowner or realtor looking to increase the market price of a home.

Type of home and style of home are associated with higher prices, just as older homes are associated with lower prices.

To isolate what features are possible to ameliorate or add without the cost surpassing the increasae in the sale price of the house, further analysis would have to be done.