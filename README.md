# Building-Energy-Model
In this project the key goal is predicting the temperature difference between indoor and outdoor using Logger sensor data 

Introduction:

Prediction of the temperature difference between indoor and outdoor is key factor in automating the HVAC system, which will optimize the building's energy and will also cut off the bills on energy. In this projec,t the key goal is predicting the temperature difference between indoor and outdoor using Logger sensor data . Machine learning regression techniques have been adopted for prediction of temperature difference .Data is extracted Amazon AWS cloud from a database named as master. Indoor data table is data that consists of records that have been collected initially we have a sensor data collected from data logger is unstructured.Building an energy model will help in creation of smart.Deep learning techniques

Data Preprocessing

Indoor data table is data which consists of records that have been collected with data logger present at the middle of the room.indoor data infront is data which consists of records that have been collected by using data loggers at the front of the data.In this project we have used only indoor and outdoor table for the prediction of temperature difference During the Preprocessing stage we have converted the type of each variables from object format to their respective formats .There were no missing values in our data.we have converted the timestamp formatinto datetime format .We have created a function which convert date and time to the bin number.Converted all the timestamps present in indoor and outdoor table into a bin number .we have merged two tables indoor and outdoor with join on bin number to make a new table which will be used prediction of temperature difference.we have plotted correlation plots to see any multicollinearity and have removed some features which are correlating very high with each other .Exploratory data analysis has been performed to find the relationship between variables

Model building

Before model building We have sampled the data to 10000 data points as some of the models are computationally expensive.rwe have built models using selected features which we have obtained from feature selection techniques.WE have also removed some of the features from the correlation plots by removing the multicollinearity between the variables Regression techniques like Linear regression ,Random forest Regressor ,SVR regressor have been adopted for prediction of temperature difference.Performed hyper parameter tuning on some of the models to perform well.We have tried PCA Analysis to improve the performance of the model but it didn't improve the performance of the model

Limitations of regression techniques

Regression techniques have some limitations as the correlation of most of features with target variables are low .All the motion variables present in the data does not have much impact on temperature difference.
-
Conclusion:
Best models that have been found are SVR Regressor and linear regression for building energy models.
Future work:
Application of Neural network and deep learning techniques for prediction of temperature difference between indoor and outdoor .NNDL techniques such as RNN,CNN,ANN can be adopted for prediction of difference between indoor and outdoor of a building
