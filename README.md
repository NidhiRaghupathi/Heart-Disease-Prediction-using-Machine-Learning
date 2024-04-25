# Heart-Disease-Prediction-using-Machine-Learning

Type of Project:
	Type of project is Classification as the target variable categorical and represents different classes. 0 and 1. 0 means person does not have heart disease and 1 means person has heart disease.

Data Import:
	Import the data using pandas library. Dataset is a csv file. Therefore pd. read_csv() is used.

Data Cleaning:
Find Null Values:
 Use isnull().sum() to see whether there are any null values . In this case there are no null values.
Find Duplicate Values:
Use duplicated().sum() to check if there are duplicate values. There was 1 duplicate row. So, use drop_duplicates() to eliminate it.
Find Outliers:
Outliers are found and eliminated using boxplot graphs.
Find incorrect values:
No incorrect values are found. It was checked by using df.info().
Data Exploration:

Describing the data columns:
Using describe() statistical information regarding the numeric features.
Understand the categorical columns:
Using various graphs various observations were made regarding dataset.
•	People having heart disease is greater than people not having heart disease. 0 =104 and 1=154.
•	People aged from 41 to 67 are more prone to heart diseases while people aged 58 are maximum affected.
•	Highest type of chest pain is “Typical Angina”.
•	Only around 25% of total count are having fasting blood sugar more than 120.
•	EXNG count is more than double for type 0
•	Thall count is max for type 2 and min for type 0.
•	There is no apparent linear correlation between continuous variable according to the heatmap.
Data Processing:
Some categorical variables need to be converted into dummy variables. For this pd.get_dummies() is used.
Data Scaling:
Some columns need to be scaled as they are in different units. So, it needs to be scaled so that all the columns are standard in nature. For this StandardScaler () is used.
Splitting the data:
Dataset must be split into training dataset and testing dataset before giving it to the machine learning model. train_test_split is used for splitting the dataset.

Model building and accuracy:
Machine learning algorithm is chosen based on the nature of the problem. In Python model is generally loaded using scikit libraries. It’s a classification problem hence logistic regression model is used.
“Model fitting" is the process of training the model on your training data. The fit() method is called on the model, and it takes the training data (x_train and y_train) as arguments.
After fitting the model, it's ready to make predictions on new, testing data.
Score of logistic regression is 84.61%.
After that Standard Vector Machine is implemented using SVC() is used .
Score of Standard Vector Machine is 83.65 %.
Random Forest algorithm is implemented using RandomForestClassifier.
Score of RandomForestClassifier is 82.69 %.
Decision Tree algorithm is implemented using DecisionTreeClassifier
Score of DecisionTreeClassifier is 76.92 %.

Observations:
Nearly all algorithms are performing well. Logistic regression is giving highest score out of few algorithms that have been used above i.e. 84.61% 

