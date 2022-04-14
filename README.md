# Predictive-Modelling-Competition

The goal of this project is to predict the number of unique objects sold in a shop over a period of 1 month using about 3 years’ worth of data. 
Given that the list of shops and products slightly changes every month, we create a robust model capable of handling these situations.
We preprocess the data to handle data noise and engineer some feature to train the models.
We then create two models: a multiple linear regression model and a Random Forest model. 
We train the models and evaluate the models performance based on the rmse.

# Step-by-step approach
• Import data into R

• Clean data by removing all NA’s and outliers.

• Pre-process shops data and categories data in Excel.
  We pre-process the shops data to get shop_city, shop_name and shop_type. We pre-process the categories data to get the item_category and item_subcategories.
  
• Add features:
  We add features like revenue, price and average total sales per month in every specific shop/specific shop type.

• Add lag features:
  We decide to use lagged sales figures from 3 prior months to help predict sales in the current month.
  
• Preparing our training and testing set:
  We use date block 0-32 (Jan 2013- October 2015) as training data set and date block 33 as the testing data set. we will compute the root mean squared error based on this testing data set.
  
 • Fitting the model:
  We go on to fit the model and compute the root mean squared error.
  
• Display the important features in the model.

• Drop unimportant features and refit the model computing the root mean squared error.

• Making sale predictions for date block 34(November 2015) using full data set.
