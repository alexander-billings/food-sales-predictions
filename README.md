Summary of the Food Sales Predictions Project
* Purpose
  * This notebook is to evaluate a machine learning model to make predictions based on data on food sales including things like price, weight, visibility in the store, etc.
* What's been done to the data
  * Duplicate rows have been deleted
  * Rows with missing data have been deleted
  * Data has been split into a set to train a machine learning model, and one to validate the training went well
* Insights
  * Low Fat Dairy produts are preferred over regular dairy products

  ![Dairy](https://github.com/alexander-billings/food-sales-predictions/blob/master/visualizations/dairy_sales_by_fat.png?raw=true)
  * Fat content does not have as strong of a correlation with snacks

  ![Snacks](https://github.com/alexander-billings/food-sales-predictions/blob/master/visualizations/snack_sales_by_fat.png?raw=true)
* Recommendations
  * Collect more sales data to include subcategories of dairy products
  * Maintain diversity of inventory in snack products
  * A Linear Regression machine learning model outperforms a Decision Tree model and should be able to predict sales using available data

Two machine learning models were evaluated: Linear Regression and Simple Decision Tree Regression. They were scored with r^2 score and RMSE score and checked for overfitting by comparing results between training and testing data.

Machine Learning Reports:

**Evaluating Linear Regression**

Training r^2 score:  0.5002893346345348
Training RMSE score: 1076.9698132655562 

Testing r^2 score:   0.5248877442594724
Testing RMSE score:  1076.68602345498


**Evaluating Decision Tree**

Training r^2 score:  0.534740727028052
Training RMSE score: 1039.1822976718233 

Testing r^2 score:   0.5370571358531255
Testing RMSE score:  1062.8076111618352


Machine Learning Recommendations:
* Use the Decision Tree model as a baseline for further evaluation
* Review data to see if there are oppurtunities for better cleaning
* Evaluate more complex models to see if they perform better

Data Dictionary:
| Variable Name	|Description|
|---|---|
|Item_Identifier	|Unique product ID|
|Item_Weight	|Weight of product|
|Item_Fat_Content|	Whether the product is low fat or regular|
|Item_Visibility	|The percentage of total display area of all products in a store allocated to the particular product|
|Item_Type	|The category to which the product belongs|
|Item_MRP|	Maximum Retail Price (list price) of the product|
|Outlet_Identifier	|Unique store ID|
|Outlet_Establishment_Year	|The year in which store was established|
|Outlet_Size	|The size of the store in terms of ground area covered|
|Outlet_Location_Type|	The type of area in which the store is located |
|Outlet_Type	|Whether the outlet is a grocery store or some sort of supermarket|
|Item_Outlet_Sales	|Sales of the product in the particular store. This is the target variable to be predicted.|