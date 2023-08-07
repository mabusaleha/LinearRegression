#### Bike-sharing-assignment
A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.

General Information
A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.

The company wants to know:
Which variables are significant in predicting the demand for shared bikes.
How well those variables describe the bike demands
Technologies Used
numpy 
pandas 
matplotlib 
plotly 
seaborn 
statsmodels
sklearn 
scipy

##### Conclusions:
1. We had a dataset with 510 records of data with the target and feature variables.
2. Performed EDA on the dataset to check for significant inferences and identify variables for data preparation. Used scatter plots for numerical and boxplots for categorical variables.¶
3. Prepared the data by converting categorical variables into dummy variables.
- season
- weathersit
- month
- weekday
- registered
4. Dropped irrelevant and categorical variables from the data.
- season
- weathersit
- month
- weekday
- instant
- dteday
- atemp
- registered
- casual
5. Split the data into test and train datasets in a 70:30 ratio.
6. Rescaled numerical variables using MinMax method.
7. Plotted a heatmap to check linearity among all the variables and identified temp to be the most significant feature.
8. Built a model using only temp feature with 41% adjusted R-Square.
9. Adopted RFE for feature selection and built 5 other models to increase adjusted R-square to 84.3%.
10. Manually identified other feature variables and built 6 other models and observed most of newly added features are having p-value > 0.05 which is insignificant.
11. Performed residual analysis to confirm assumption of residuals hold true.
12. Made predictions on the train data.
13. Evaluated the model on test data with 81.5 % accuracy.
