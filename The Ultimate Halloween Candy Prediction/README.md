# THE ULTIMATE HALLOWEEN CANDY POWER RANKING
![datasetcover](https://raw.githubusercontent.com/hnlgangte/MachineLearning-with-Python/main/The%20Ultimate%20Halloween%20Candy%20Prediction/images/candy.jpg "datasetcover")

The goal is to create a model using the provided predictor variables for predicting of the overall win percent of candy and evaluate the model using possible model evaluation techniques.
# Data  Description
What 

is the best (or at least the most popular) Halloween candy? That was the question this dataset was collected to answer. Data was collected by creating a website where participants were shown presenting two fun-sized candies and asked to click on the one they would prefer to receive. In total, more than 269 thousand votes were collected from 8,371 different IP addresses.
The dataset comprises of 85 rows and 13 columns.
For binary variables, 1 means yes, 0 means no. The data contains the following fields:

|Feature||Description|
|-------||-----------|
|chocolate|	|Does it contain chocolate?|
|fruity|	|Is it fruit flavored?|
|caramel|	|Is there caramel in the candy?|
|peanutalmondy:||	Does it contain peanuts, peanut butter or almonds?|
|nougat|	|Does it contain nougat?|
|crispedricewafer||	Does it contain crisped rice, wafers, or a cookie component?|
|hard||	Is it a hard candy?|
|bar||	Is it a candy bar?|
|pluribus||	Is it one of many candies in a bag or box?|
|sugarpercent||	The percentile of sugar it falls under within the data set.|
|pricepercent||	The unit price percentile compared to the rest of the set.|
|winpercent||	The overall win percentage according to 269,000 matchups.|
## Exploratory Data Analysis
![corrmap](https://raw.githubusercontent.com/hnlgangte/MachineLearning-with-Python/main/The%20Ultimate%20Halloween%20Candy%20Prediction/images/heatmap.png "corrmap")
###### By establishing Correlation between features using heatmap it is observed that-
- Makers do not mix chocolate and fruits most of the time.
- Candies which are shaped as bar generally has chocolate and/or nougat and they are least likely to be in a bag and have fruits.
- Chocolate means win (mostly).
- Sugar doesn't have a considerable effect on winning.

##### Feature Importance of Various Attributes
![feature](https://raw.githubusercontent.com/hnlgangte/MachineLearning-with-Python/main/The%20Ultimate%20Halloween%20Candy%20Prediction/images/feature.png "feature")
## CONCLUSION
We have built and compared the performance of three models using various model evaluation metrics. The performance of the three models using different regressor algorithims based on various model evaluation metrics are shown below:

|   | MAE  | MSE  |  RMSE |  R2 |Adj. R2   |
| ------------ | ------------ | ------------ | ------------ | ------------ | ------------ |
|LR   | 10.464152742303979  |  167.05181735247982 | 12.924871728728334  | 0.5855129919383147  | 0.5040959010690551  |
|DT  | 11.42488791911765  | 198.44806471767498  | 13.559106546254178  |  0.9214810923504617 |  0.906057735490731 |
|RF   |10.310102389741173   | 166.95379560889467  | 12.741095954256782  |0.9167856180272164   |0.900439935853991   |

Since our Objective is to minimize the prediction errors so that the model predicts more accurately. Therefore, among the various regression metrics, we give more importance to RMSE.

As RMSE value of Random Forest Model is the least compared to models built with Linear Regression and Decision Tree, the Random Forest model is most preferable.
