# House-Price-Prediction
House price prediction using Linear regression

This is a famous data set for beginners practicing regression. In this program, I will implement multivariate linear regression to predict the "Sale prices" of houses.

# Which DataSet is this?:
[Armes Housing Dataset](http://jse.amstat.org/v19n3/decock.pdf) is an alternative to commonly used Boston Housing dataset.


# What you would need to run .ipynb file?
Jupyter Notebook from Anaconda distribution


# What libraries are used in the code?
scikitlearn, pandas, numpy and matplotlib.


# Well, something more about the dataset?
This housing dataset contains 80 variables, Among them, 57 are categorical variables and 23 are numerical variables.

train.csv contains 1460 rows and test.csv contains 1459 rows.

Description of variables is as follows:
SalePrice - the property's sale price in dollars. This is the target variable that you're trying to predict.
MSSubClass: The building class
MSZoning: The general zoning classification
LotFrontage: Linear feet of street connected to property
LotArea: Lot size in square feet
Street: Type of road access
Alley: Type of alley access
LotShape: General shape of property
LandContour: Flatness of the property
Utilities: Type of utilities available
LotConfig: Lot configuration
LandSlope: Slope of property
Neighborhood: Physical locations within Ames city limits
Condition1: Proximity to main road or railroad
Condition2: Proximity to main road or railroad (if a second is present)
BldgType: Type of dwelling
HouseStyle: Style of dwelling
OverallQual: Overall material and finish quality
OverallCond: Overall condition rating
YearBuilt: Original construction date
YearRemodAdd: Remodel date
RoofStyle: Type of roof
RoofMatl: Roof material
Exterior1st: Exterior covering on house
Exterior2nd: Exterior covering on house (if more than one material)
MasVnrType: Masonry veneer type
MasVnrArea: Masonry veneer area in square feet
ExterQual: Exterior material quality
ExterCond: Present condition of the material on the exterior
Foundation: Type of foundation
BsmtQual: Height of the basement
BsmtCond: General condition of the basement
BsmtExposure: Walkout or garden level basement walls
BsmtFinType1: Quality of basement finished area
BsmtFinSF1: Type 1 finished square feet
BsmtFinType2: Quality of second finished area (if present)
BsmtFinSF2: Type 2 finished square feet
BsmtUnfSF: Unfinished square feet of basement area
TotalBsmtSF: Total square feet of basement area
Heating: Type of heating
HeatingQC: Heating quality and condition
CentralAir: Central air conditioning
Electrical: Electrical system
1stFlrSF: First Floor square feet
2ndFlrSF: Second floor square feet
LowQualFinSF: Low quality finished square feet (all floors)
GrLivArea: Above grade (ground) living area square feet
BsmtFullBath: Basement full bathrooms
BsmtHalfBath: Basement half bathrooms
FullBath: Full bathrooms above grade
HalfBath: Half baths above grade
Bedroom: Number of bedrooms above basement level
Kitchen: Number of kitchens
KitchenQual: Kitchen quality
TotRmsAbvGrd: Total rooms above grade (does not include bathrooms)
Functional: Home functionality rating
Fireplaces: Number of fireplaces
FireplaceQu: Fireplace quality
GarageType: Garage location
GarageYrBlt: Year garage was built
GarageFinish: Interior finish of the garage
GarageCars: Size of garage in car capacity
GarageArea: Size of garage in square feet
GarageQual: Garage quality
GarageCond: Garage condition
PavedDrive: Paved driveway
WoodDeckSF: Wood deck area in square feet
OpenPorchSF: Open porch area in square feet
EnclosedPorch: Enclosed porch area in square feet
3SsnPorch: Three season porch area in square feet
ScreenPorch: Screen porch area in square feet
PoolArea: Pool area in square feet
PoolQC: Pool quality
Fence: Fence quality
MiscFeature: Miscellaneous feature not covered in other categories
MiscVal: $Value of miscellaneous feature
MoSold: Month Sold
YrSold: Year Sold
SaleType: Type of sale
SaleCondition: Condition of sale

# How were the features transformed before fitting the model?
From my initial exploratory analysis most of the variables are skwed datasets, i.e, their mean and medians differ. Hence, I chose to do log transformation so that the variables will be approximately normal.If at all the data was not skewd, I could have gone with standard guassian transformation.

Also as I must, I have one-hot encoded the categorical variables such that, I can use them in my linear regression model.

Dataset had 14 numerical variables which are actually categorical like for example, month of the year. I have identified them and onehotencoded them as well.


# which linear regression is used?

I have used Linear regression with gradient descent to find the best coefficient values of the predictors.
I have applied Ridge(L2) and Lasso(L1) regularizations to reduce the overfitting effect of too many variables.


# How was the score improved? How are the hyperparameters selected?

The only hyperparameter in case of lienar regression is the regularization paramter. 
The best tregularization paramter is estimated as the one that performed best across cross validation datasets.


# what did we achieve from running this model?

Low Overall quality index and less pool area negatively effect the sale price of the house.

High Overall quality rating of 10,9 and neighborhoods of Crawfor and StoneBr are postively associated with high sale prices.

By how much these variables effect the house sales price can be calculated by substituting our estimated coefficients values in the regression equation.


# House Price Prediction(Regression) with Tensorflow - Keras

<img src="/house.jpg" width="1000" height="300" />
<div align="justify">

## Tensorflow and Keras
**TensorFlow** is an end-to-end open source platform for machine learning. It has a comprehensive, flexible ecosystem of tools, libraries and community resources that lets researchers push the state-of-the-art in ML and developers easily build and deploy ML powered applications.<br /><br />
**Keras** is an open-source neural-network library written in Python. It is capable of running on top of TensorFlow, Microsoft Cognitive Toolkit, R, Theano, or PlaidML. Designed to enable fast experimentation with deep neural networks, it focuses on being user-friendly, modular, and extensible.

## Dataset

The data contains information from the 1990 California census. The columns are as follows:<br />
*longitude:* A measure of how far west a house is; a higher value is farther west<br />
*latitude:* A measure of how far north a house is; a higher value is farther north<br />
*housingMedianAge:* Median age of a house within a block; a lower number is a newer building<br />
*totalRooms:* Total number of rooms within a block<br />
*totalBedrooms:* Total number of bedrooms within a block<br />
*population:* Total number of people residing within a block<br />
*households:* Total number of households, a group of people residing within a home unit, for a block<br />
*medianIncome:* Median income for households within a block of houses (measured in tens of thousands of US Dollars)<br />
*medianHouseValue:* Median house value for households within a block (measured in US Dollars)<br />
*oceanProximity:* Location of the house w.r.t ocean/sea<br /><br />

Data Source: [California Housing Prices Dataset](https://www.kaggle.com/camnugent/california-housing-prices/version/1)

</div>
