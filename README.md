# Predicting House Prices

A data science project that takes raw data and makes a model to predict house prices 

The model chosen is a linear regression model which was further improved by Tikhonov regularization-or commonly known as Ridge Regression. 

Structurally, there are two parts of it:
* Data wrangling (or cleaning) and Exploratory Data Analysis
* Model building and evalution

The dataset is a modified version of [this Kaggle Dataset](https://www.kaggle.com/harlfoxem/housesalesprediction). 

# Dataset

This dataset contains house sale prices for King County, which includes Seattle. It includes homes sold between May 2014 and May 2015.

Here's a summary of the columns:

__id__ : A notation for a house

__date__: Date house was sold

__price__: Price is prediction target

__bedrooms__: Number of bedrooms

__bathrooms__: Number of bathrooms

__sqft_living__: Square footage of the home

__sqft_lot__: Square footage of the lot

__floors__ :Total floors (levels) in house

__waterfront__ :House which has a view to a waterfront

__view__: Has been viewed

__condition__ :How good the condition is overall

__grade__: overall grade given to the housing unit, based on King County grading system

__sqft_above__ : Square footage of house apart from basement

__sqft_basement__: Square footage of the basement

__yr_built__ : Built Year

__yr_renovated__ : Year when house was renovated

__zipcode__: Zip code

__lat__: Latitude coordinate

__long__: Longitude coordinate

__sqft_living15__ : Living room area in 2015(implies-- some renovations) This might or might not have affected the lotsize area

__sqft_lot15__ : LotSize area in 2015(implies-- some renovations)

## The Notebooks
The notebooks go through the entire process of model development. It includes: 
* Data Wrangling
    - Removing problematic data
    - Taking care of NA Values
    - Saving multiple versions of incrementally cleaned data
* Exploratory Analysis
    - Finding correlation with Pearson's coefficient
    - Using scatterplots and boxplots to find relationships with the target variabless
    - Using p-value to check for statistical significance
* Multiple Linear Regression Model
    - Building model
    - Evaluating using metrics such as R-squared
* Polynomial Regression
    - Using Polynomial Features
    - Creating a pipeline
    - Evaluation
* Ridge Regression
    - Tuning Hyperparam 
* k-fold Cross Validation
* Conclusion
