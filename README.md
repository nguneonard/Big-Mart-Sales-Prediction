# Big-Mart-Sales-Prediction

## Project Objective
The purpose of this project is to build a predictive model to find out the sales of each product at a particular store at BigMart.
This helps the decision makers to find out the properties of any product or store, which play a key role in increasing the overall sales.
Using this model, we will try to understand the properties of products and outlets which play a key role in increasing sales. Lightgbm gave the 
best model accuracy of 60% and least absolute error and was therefore used to deploy our model.

## Project Description
The goal of this project was to build a predictive model capable of predicting sales of products at the various stores in Big Mart. 
After brainstorming on the objectives, it was then time to acquire the data. The data for this project is available at:


train file:https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/download/train-file
test file:https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/download/test-file
sample submission file:https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/download/sample-submission

## Dataset Description
| Variable     | Description |
| -----------  | ---: |
|Item_Identifier | Unique product ID|
|Item_Weight | Weight of product|
|Item_Fat_Content | Whether the product is low fat or not|
|Item_Visibility | The % of total display area of all products in a store allocated to the particular product|
|Item_Type | The category to which the product belongs|
|Item_MRP | Maximum Retail Price (list price) of the product|
|Outlet_Identifier | Unique store ID|
|Outlet_Establishment_Year|The year in which store was established|
|Outlet_Size|The size of the store in terms of ground area covered|
|Outlet_Location_Type|The type of city in which the store is located|
|Outlet_Type|Whether the outlet is just a grocery store or some sort of supermarket|
|Item_Outlet_Sales|Sales of the product in the particular store. This is the outcome variable to be predicted.|

The dataset description if found in the notebook.
Looking/going through the data, i had to come out with some ***hypothesis*** to guide me in analysis as follows:
- Item weight might effect a sales of the product.
- Sales of the product may be depends on the items fat content.
- More Item_Visibility of a particular product may be costlier than other products.
- Item type could have an effect on the sales.
- Are the items with more MRP have more item outlet sales.
- Are the stores which have established earlier have more sales.
- Size of the stores could have an effect on the item sales at a particular store.
- Location of the stores might depends on the Item outlet sales.
- Are the supermarkets have more sales than others.

The answers to these questions were verified by performing exploratory data analysis on the dataset notably: univariate and bivariate analysis in order
to view some hidden inside of the data.Then we proceed unto data preprocessing where missing data and outlier analysis was performed. Going through the notebook, we will realise that the train and test dataset were concatenated before performing the appropriate cleaning so as to avoid the redundant work of cleaning train and test dataset separately.Since machine learning algorithms work only with numbers after the cleaning the process, i performed one-hot encoding to convert the rest of the categoricalmvariables to numerical variables and subsequent dropping of irrelevant features. This was followed by applying various regression models using scikit learn andcomparing the accuracy of each. The best model was then tuned using grid_search and finally applied in the test dataset.

## Methods Used
- Machine Learning
- Data Visualization
- Predictive Modeling
- feature engineering
- Inferential Statistics

## Technologies used
- seaborn
- matplotlib
- numpy
- scikit learn
- pandas

## Needs of this project
- data exploration/descriptive statistics
- data processing/cleaning
- feature engineering
- statistical modeling

## Contributing DSWG Members

**Team Leads (Contacts) : [Kubin Ngu Neonard](https://github.com/nguneonard)**
