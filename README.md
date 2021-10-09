# food-sales-prediction

For my first data science project, I was given a large dataset with information about products and the outlet stores they are sold in. Features of this dataset included item identifiers, item weight, item type,  item MRP, outlet identifier, outlet size, outlet type,  item outlet sales, and more. The goal was to use this dataset to understand trends in the data and make sales predictions.

This project is broken up into 6 steps: 
1. Basic notebook setup: Importing the necessary libraries and creating a DataFram using pandas. Using the .head() function to examine the features and values of the first few rows of the dataframe.
2. Data cleaning: Checking the dataframe shape and datatypes, checking for and addressing any duplicate rows, missing values, and inconsistent categories, and producing summary statistics of each numerical category (min/max/mean)
3. Statistical analysis: Creating visualizations such histograms, boxplots, and correlations.

Histogram showing distribution of item count across individual outlets

![image](https://user-images.githubusercontent.com/89666293/136664786-f33eedd6-61b4-4de8-9e65-28fd8d135709.png)

Histogram comparing distributions of item types in stores established in 1985 and 2009, which were the oldest and newest stores in the dataset respectively

![image](https://user-images.githubusercontent.com/89666293/136664800-a08ea880-7736-4a79-a035-3b67cac53a02.png)

Boxplots to view statistical summaries of item weights and summaries of item outlet sales by individual outlets

![image](https://user-images.githubusercontent.com/89666293/136664809-0a3c7351-b6a5-48dd-aa6b-0d67e9921824.png)
![image](https://user-images.githubusercontent.com/89666293/136664812-b1ec077f-7359-487f-a8d5-72fc65e58420.png)

Heat map to see the correlation between features. The strongest correlation shown here is between item outlet sales and item MRP.

![image](https://user-images.githubusercontent.com/89666293/136664819-b46b116d-af4a-4a91-b76d-748d1ad3e048.png)

4. Explanatory Analysis: Building data visualizations to better understand trends in the data. 

Bar chart illustrating the highest and lowest sales at a specific outlet (snack foods and seafood items were highest and lowest, respectively).

![image](https://user-images.githubusercontent.com/89666293/136664855-5c920f5a-aac6-4eb4-895c-890b47c984f1.png)

Bar char illustrating that Outlet 27 had the highest item sales among medium sized stores.  Owners of these other outlets may want to look closer at Outlet 27 data and see what they can do to improve their sales.

![image](https://user-images.githubusercontent.com/89666293/136664959-a8364bf9-168f-4942-b50d-e304c333d0f1.png)


5. Linear Regression: Transforming the categorical variables into numbers and use dummy encoding, one hot encoding, and hashing where appropriate. Using models to predict sales. Evaluating the test set results using R^2 and RMSE

6. Tree based models: building a decision tree model, a bagged tree model, and a random forest model. Comparing the R^2 and RMSE scores to determine which model would be best to use.

Recommendation: Retailers should create sales predictions on this dataset using the Random Forest Model because it had the lowest RMSE and highest R^2 scores of the different models evaluated.

