# House-Price-Prediction
House price prediction using MUltiple Linear regression and Keras Regression

This is a famous data set for beginners practicing regression. In this program, I will implement multivariate linear/keras regression to predict the "Sale prices" of houses.

# Which DataSet is this?:
[Bangalore Housing Dataset](https://www.kaggle.com/amitabhajoy/bengaluru-house-price-data) is an alternative to commonly used Boston Housing dataset.


# What you would need to run .ipynb file?
Jupyter Notebook from Anaconda distribution

# What libraries are used in the code?
scikitlearn, pandas, numpy and matplotlib.

# Well, something more about the dataset?
This housing dataset contains above 40 variables, Among them, 37 are categorical variables while rest are numerical variables.
train.csv contains 1460 rows and test.csv contains 1459 rows.

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

# which linear regression is used?
I have used Linear regression with gradient descent to find the best coefficient values of the predictors.

## Tensorflow and Keras
**TensorFlow** is an end-to-end open source platform for machine learning. It has a comprehensive, flexible ecosystem of tools, libraries and community resources that lets researchers push the state-of-the-art in ML and developers easily build and deploy ML powered applications.<br /><br />
**Keras** is an open-source neural-network library written in Python. It is capable of running on top of TensorFlow, Microsoft Cognitive Toolkit, R, Theano, or PlaidML. Designed to enable fast experimentation with deep neural networks, it focuses on being user-friendly, modular, and extensible.

# How was the score improved? How are the hyperparameters selected?

The only hyperparameter in case of lienar regression is the regularization paramter. 
The best tregularization paramter is estimated as the one that performed best across cross validation datasets.


# what did we achieve from running this model?

Low Overall quality index and less pool area negatively effect the sale price of the house.

High Overall quality rating of 10,9 and neighborhoods of Crawfor and StoneBr are postively associated with high sale prices.

By how much these variables effect the house sales price can be calculated by substituting our estimated coefficients values in the regression equation.

