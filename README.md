"""# Conclusion:
- data has high number of outliers as a result positive  Skewed
- target feature is highly enbalenced need to be handeld properly 
- there is multicolenearty in data 
- the amount of data is big we need to handle data so the training and prediction time can be saved 
"""


# my aopproch 
- I converted csv into parquet then removed unnececery column,change the data type of some column to int8 from defult int64 to save memory uses this was the most chalenging thing in my my approch.
- By useing less memory i was able to get rendom forest 5 k fold cross validation time from 4 hours to hour to finally around 20 minutes.  
- Also i uesed smote to  balance imbalance data from imbalance librery
- to privent over fitting i used simple models also used k fold cross 
- i also did hyper perameter tuning with GridSearchCV
- and finally used sklearne pipeline to do data transformation during prediction


# data set 
- data set is available at kaggle under the name "PS_20174392719_1491204439457_log.csv"
