# Ames, Iowa Housing: Data Cleaning, Feature Engineering, Predictions, and Kaggle Competition

# Problem Statement

Zillow will often indicate 'Estimated Home Price' to inform users about the market rates of homes, even if they are not yet explicitly for sale. More accurate depictions of home values translates to confidence in Zillow's product, and, therefore, user base expansion.

Build a Multiple Linear Regression Model that will make the best possible predictions of home values in Ames, Iowa using the provided dataset from Zillow. The model will be evaluated using an r-squared score as well as cross val score. 

Users could effectively utilize our model to predict home values and increase confidence in estimated home costs.

# Executive Summary

The importance of proper data cleaning, munging, wrangling, manipulation cannot be overstated. The preponderance of data columns, or features, the amount of errors or null values, required careful selection and aggregation in order to arrive at accurate housing price predictions. 

# Contents:

- [Data Dictionary](#Data-Dictionary)
- [Conclusions and Recommendations](#Conclusions-and-Recommendations)

## Data Dictionary

A data description was provided and can be found here: http://jse.amstat.org/v19n3/decock/DataDocumentation.txt

All features listed below were engineered for both training and testing datasets.

|Feature|Type|Description|
|---|---|---|
|**age**|*int*| Age of the house when it was sold 
|**total_fin_sf**|*int*| Total living area 'under HVAC' 
|**total_baths**|*float*| Total number of bathrooms including half-baths (0.5)
|**good_features**|*float*| Count of good or positive features 
|**bad_features**|*float*| Count of bad or negative features

## Conclusions and Recommendations:

#### Having a clear goal while feature engineering, data munging, and modeling are the key to accurate results with this dataset. Knowing what features were important and how to leverage them to have an affect on the target helped immensely. Grouping or clumping features together was fruitful and will be used again for other projects of this magnitude. Models where we utilized our engineered features fared much better than ones using only one variable. Creating dummy variables and scaling our variables also increased the accuracy of our predictions. 
#### Deliberately avoiding features that are inherently problematic, such as zip code or neighborhood, prevent our models from having a sociological bias. 
#### Future projects with this dataset could include using other models besides linear regression such as Ridge/Lasso/Elastic Net and utilizing a pipeline to deploy each of these hyperparameter tuners. 