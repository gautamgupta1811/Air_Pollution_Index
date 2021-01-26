# Air Pollution Index
 This repository conatins code for HackerEarth Machine Learning challenge: Calculate the air pollution index
   
## Approach
In this Machine Learning model for Air Pollution Index Prediction, Multiple Regression is used. After loading and analyzing the Training and Testing data, the ‘date_time’ column is dropped from training as well as the testing data.   
Different Categorical features including ‘is_holiday’ and ‘whether_type’ are grouped together with the mean of air_pollution_index(API). The groups are then sorted in the ascending order of the API. Based on the amount of variation in the values of API, the numerical values are assigned to the groups. In short, the Ordinal Approach is followed for assigning the numerical values to categorical features. Thus, all the categorical features are converted into numeric form and the data set is prepared to train the model. Similar conversions are also applied to the test dataset.  
Scikit-learn linear_model package is used for training the model. The Reg variable consists of trained data weights. These weights are used for making further predictions on x_test which comprises test data frame values. After the training of the model, predictions are stored in the Data Frame consisting of timestamps along with prediction values. This Data frame is then converted to a CSV file for further reference.  
Pandas Module is used for loading and performing all the analyses over Train data as well as Test data. Different functions such as read_csv, group_by, DataFrame are used for loading, grouping, and creating Data Frames. Many Dataframe functions are also used for analyzing, cleaning, and manipulating the data.   
  
For predicting the values, the Scikit Learn module is used. The Linear Regression function from the Linear_Model is used for fitting the data as well as predicting the values.  
  
For making predictions over different datasets, the path for the new dataset needs to be set in the cell where data is loaded. After running the complete kernel predicted values are stored in file name predictions.csv which is created in the current working directory.  

