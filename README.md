# Regression_model_comparison_for_price_prediction
"Machine Learning (ML) is crucial in modern business and research, automating decisions through algorithms and neural networks. In real estate, valuation challenges persist without robust detection methods. ML trains models for accurate predictions, enhancing decision-making and addressing these issues for all stakeholders."

Explanation of Dataset: 
First of all, we have nine features in our dataset and 13000 records and price is the main feature 
that we have to predict and it is also called the class attribute and the other features are:
1) Area Type
2) Location
3) Availability
4) Size
5) Society
6) Balcony
7) Bath
8) Total_sqft
9) Price

    
In Area type feature we have different we have different areas such as Super Built-up are and plot area and also there is a society feature that have different societies like Jades, Soiewre,
Coomee, Theanmp and also there is the other feature size which tells us that how many roomsare there in the house and also No of bathrooms is the feature and total square feet of the house 
is the main feature that tells us the house covers how much area and also the other feature is balcony that how many balconies are present and location feature in the data set is very 
important because it affects the price much more than the other feature and availability is also an other feature but according to me it is not very important feature in predicting the price.
Also, in our data set we have null values and too much large values which are called outliers and they affect the price feature and our prediction will be wrong. So, before predicting the 
price we perform “Data Pre-Processing” and through this we clean our data by removing the null values and outliers by outlier detection and also do the dimensionality reduction and at 
last from the clean data build a model and perform analysis on different types of machinelearning model and check that which will gives the best score values and who will predict the 
price better and accurate.Also, the data set we choose is of the Bengaluru city and of different locations and differenthome prices information is present in dataset.

Data Preprocessing: 
Data preprocessing is a step in the data mining and data analysis process that takes raw data and transforms it into a format that can be understood and analyzed by computers and machine learning. Raw, real
world data in the form of text, images, video, etc., is messy. Not only may it contain errors and inconsistencies, but it is often incomplete, and doesn’t have a regular, uniform design. Machines like to process nice and tidy information they read data as 1s and 0s. So, calculating structured data, like whole numbers and percentages is easy. However, unstructured data, in the form of text and images must first be cleaned and formatted before analysis.

Importance of Data Preprocessing: 
When using data sets to train machine learning models, you’ll often hear the phrase “garbage in, garbage out” This means that if you use bad or “dirty” data to train your model, you’ll end up with a bad, improperly trained model that won’t actually be relevant to your analysis. Good, preprocessed data is even more important than the most powerful algorithms, to the point that machine learning models trained with bad data could actually be harmful to the analysis you’re trying to do giving you “garbage” results.


Data Cleaning: 
We are using supervised learning and we use on data set basically the input and output value.Libraries like pandas are basic block for cleaning the data. Import basic libraries like python, 
matplotlib and NumPy. Matplotlib is a comprehensive library for creating static, animated, and interactive visualizations in Python. 
NumPy supports a wide range of hardware and computing platforms, and plays well with distributed, GPU, and sparse array libraries

Feature Engineering: 
We are copying the data frame into a new data frame by using copy () function. We are doing 
the feature engineering to make the other steps further easy. So, to check we are finding unique 
location by calling the location. unique () function and grouping it by calling the dfs. groupby
() function for the location with aggregation function.
Also, we made a new feature here which is price per square feet.


Outlier Detection: 
We are just detecting and then removing the outliers, sometimes they are just not data errors 
but also, they are causing extreme variation in the dataset. We are using different techniques 
to detect the outliers like STANDARD DEVIATION or SIMPLE DOMAIN KNOWLEDGE.


Model Building: 
We are building the machine learning model and then using the K fold cross validation and 
grid search CV to come up with the best algorithm and the best parameter.
Machine learning model can’t interpret the text data. So, we have a text data in our data set
(location) and we have to convert it into the numeric values. 
We are using the pandas dummy model to do it, the function called is like pd.get_dummies
(df10.location). as the feature location is having the data in the form of text so this function
will convert this data into the numeric values. When we have the 1st location, all the column 
will be 1 and every other value in data set is zero.



