# Cafe
Analysis data of Cafe and making prediction with two models to Predict the quantity that will be sold


### Our main problem 
we're trying to focus on revolves around quantity, whether it's the quantity sold in the past and has data, or the quantity to be sold in the future and what if we increase the price per quantity.
Therefore, we have analyzed the relationships between the quantity and other features to identify the factors that positively or negatively affect it. By focusing on the positive factors, we can enhance the quantity, while minimizing the negative factors to reduce their impact on the quantity.
We have also developed a model that predicts the quantities based on different features.
We did not develop just one model, but two models to compare and achieve the lowest error and highest accuracy. The two models are linear regression and decision tree.

                                                                                                                                                                                                          
## Steps we did in this project
### import libraries 
1- pandas and Numpy for data manipulation                                                                                                     
2- matplotlip and seaborn for data visualization                                                                                               
3- sklearn with its modules and function for linear regression model and decision tree                                                                                                                                                                                                          

### data preprocessing
1- merge data                                                                                                                                 
2- check duplicates                                                                                                                           
3- check nulls                                                                                                                            
4- get a column of (CALENDAR_DATE) in its good type.                                                                                           
5- extract columns of day, month, and week from column(CALENDAR_DATE)                                                                         
6- segment the price into 6 categories.                                                                                                      
7-drop unneeded columns.                                                                                                                           
                                                                                                     
                                                                                                     
### EDA                                                                                                                                       
1- heatmap to know the relations                                                                                                               
2- explore some features                                                                                                                       
3- relationship between quantity and another features like (IS_OUTDOOR , price , IS_WEEKEND , AVERAGE_TEMPERATURE ,
                                                                             sell id , YEAR , holiday,week)                                   
4- relationship between sell_id and price                                                                                                     
5- distribution of day and weeks and months                                                                                                   
6- Some three-features relationships                                                                                                                           
                                                                                                     
                                                                                                     

### Model 1 ( Linear regression model )                                                                                                       
1- split data in features and target ( quantity )                                                                                             
2- split the features and target in train and test with 25 % for test                                                                         
3- call linearRegression() function from sklearn                                                                                             
4- fit the train data                                                                                              
5- test the test data                                                                                             
6- check the accuracy with (0.81)                                                                                             
7- plot scatter plot and the linear regression model.                                                                                         
8- make evaluation matrix ( mean_squared_error , explained_variance_score , r2_score , mean_absolute_error )                                   
9- data validation                                                                                                                             
##### under fitting happened in Linear regression model because data shape (5420, 12)                                                         
##### so we cannot get prediction of new values by linear regression model and tring descion tree

                                                                                                     
                                                                                                     

### Model 2 ( Decision Tree model )
1- split data in features and target ( quantity )                                                                                             
2- split the features and target in train and test with 20 % for test                                                                         
3- call  DecisionTreeRegressor() function from sklearn                                                                                         
4- fit the train data                                                                                                                         
5- test the test data                                                                                                                         
6- check the accuracy with (0.95)                                                                                                            
7- plot scatter plot and the linear regression model.                                                                                         
8- make evaluation matrix ( mean_squared_error , explained_variance_score , r2_score , mean_absolute_error )                                   
##### in Decision Tree model Data validation is more sense than regression model because the desion tree more fitted to the small data
##### so we decided to use this model to make prediction by it 

                                                                                                     
                                                                                                     

## problems we faced 
1- data in more than one files and not all common features                                                                                     
2- the is no feature common that could we can get from it categoery name                                                                       
3- more data needing as because of data has only 5000 raw underfitting happened                                                                                             

