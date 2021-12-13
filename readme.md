# Predictive Data Analytics on Health Care Reform
## Purpous
This was a group project done for my Fundamentals of Data Science class. Our goal was to do Predictive Data Analytics using a Health Care Reform Dataset. This included predicting features like: A persons political beliefs and their opinions on the health care system in the United States.
## Process
To do this we followed the CRISP-DM process. We started with out raw data. Then processed it doing things like Data Cleaning and building summary tables to analyze our features. From here we went to modeling and then to evaluation.
## Modeling
Our data was mainly categorical features because of this we had to pay close attention to the type of methods we used.
### Feature Selection
Since we had a large number of features the only way to reduce the data was to use a feature selection algorithm. We chose to use chi squared feature selection because our data was categorical.
### DNN
We tested multiple predictive algorithms for predicting our target features but the most effective was the Deep Neural Network. This was constructed using TFlearn. There are a lot of specifications when it comes to our DNN so going through them all is difficult but here is a short summary.
#### Ordinal Target Feature
Since our goal was to predict ordinal target features we had to tune the DNN to be able to work with this. To put this into a form that the model could work with we had to ordinally encode our target feature. We also had to use the Sigmoid activation function for our output layer as a result of the ordinal target feature. For our loss function we had to use categorical cross entropy as a result of this too.
#### Optimizing loss
Origionally we had set our epoch to be 100. When we did this our accuracy was rather low. After optimizing epoch through analyzing loss data we saw a drastic increase in our accuracy. Over all the accuracy was around 89%.
## Files
Our repo is a little messy but here are some of the main files that where used. Data_Cleaning was used for our data cleaning. Encode_Feature_Selection is what was used for encoding our dataset and doing feature selection. Then our DNN can be found in AI_IDEOLOGY5.
