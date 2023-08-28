# Covid-Cases-prediction-using-ML
The aim was to predict the Total Covid cases which may occur on a particular unknown test vector and to create a ML model with higher accuracy as much as possible.
Tasks performed:
● Extracted and understood the dataset containing Covid cases , related deaths and Hospital beds available for all Countries.
Conducted data preprocessing tasks, including handling missing values and scaling the features.
● For Null values in Continuous Numerical columns, they were replaced with Total Mean of that column.
● For Null values in Ordinal Numerical columns, they were replaced with Total Mode of that column.
● For Null values in Categorical columns, they were replaced with Mode of that column.
● If there were any columns where more than 50 percent of the values are Null then those columns were dropped from the Dataset.
● Implemented Univariate Analysis, a total of 10 feature columns were selected and Histograms were plotted for each one of them using matplotlib python library. Calculated the total Mean, Median and Mode of each Feature column for better understanding.
● Implemented Bivariate Analysis, Scatter plots and Line plots were plotted for all the Target columns against the Target Feature (“Total cases” column) with the help of matplotlib python library.
● Converted the Date column from Timestamp format to ordinal because Machine Learning algorithms can be used on feature columns only if they are either continuous, ordinal.
● Dropped useless Categorical columns such as Country Code, Country, Continent because in predicting the number of Covid cases the information given by these columns serve no purpose. The useful ones are converted from Categorical to Numerical.
● Developed and trained a Machine Learning model using the regressor algorithms Linear Regression, Random Forest Regressor from the “Sci-kit Learn” python library. Calculate the Accuracy for each algorithm.
● Predicted “Total cases” target column numerical values for new Row vectors.
● Utilized evaluation metrics such as precision, recall, and F1-score to assess the model's performance.
● Collaborated with the assigned team to integrate the developed model into the existing covid cases prediction system.
Output : The accuracy score of Test data (30 percent of whole dataset) were successfully calculated for two ML algorithms after successful data pre-processing techniques. Firstly, Linear Regressor was used which gave around 98 percent accuracy, similarly the Random Forest Regressor was used which had 99 percent accuracy. Hence from the above result, clearly both the ML algorithms can be used for accurate predictions of target values as the accuracy values are almost the same. A sample row vector was taken as input and the Total COVID cases target column was found using predict method of both Linear and Random Forest regressor where the error deviation was about 15 percent from the accurate value.
