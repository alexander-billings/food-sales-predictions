Summary of the Food Sales Predictions Project
* Purpose
  * This notebook is to evaluate a machine learning model to make predictions based on data on food sales including things like price, weight, visibility in the store, etc.
* What's been done to the data
  * Duplicate rows have been deleted
  * Rows with missing data have been deleted
  * Data has been split into a set to train a machine learning model, and one to validate the training went well
* Insights
  * Low Fat Dairy produts are preferred over regular dairy products
  * Fat content does not have as strong of a correlation with snacks
* Recommendations
  * Collect more sales data to include subcategories of dairy products
  * Maintain diversity of inventory in snack products
  * A Linear Regression machine learning model outperforms a Decision Tree model and should be able to predict sales using available data

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