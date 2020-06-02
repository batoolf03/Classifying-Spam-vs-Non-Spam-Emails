# Classifying-Spam-vs-Non-Spam-Emails
Dataset: http://archive.ics.uci.edu/ml/datasets/Spambase.Specifically, 
- (i) file “spambase.data” contains the actual data
- (ii) files “spambase.names” and “spambase.DOCUMENTATION” contain the description of the data. 
This dataset has 4601 records, each record representing a different email message. Each record is described with  58  attributes  (indicated  in  the  aforementioned  .names  file):  attributes  1-57  represent  various  content-based characteristics already extracted from each email message (related to the frequency of certain words or certain punctuation symbols in a message as well as to the usage of capital letters in a message), and the last attribute represents the class label for each message (spam or non-spam). 
Task: The general task for this assignment is to build two different models for detecting spam messages (based on  the  email  characteristics  that  are  given): 
- (i)  the  best  possible  model  that  can be built in  terms  of  the overall predictive accuracy (i.e., not taking any cost information into account)
- (ii) the best cost-sensitive classification model that you can build in terms of the average misclassification cost. 

## Algroithms considered - 
- Decision Tree: No need to do feature selection for DT as it automatically adjusts for outliers and picks the most relevant features 
- Logistic Regression: Drop variables that are highly vorrelated and then use the rest for L1 which will conduct feature selection automatically 
- KNN: Two way of going about KNN. i)Use Logistic regression's best output with the most relevant features selected. ii) execute one iteration with all features included
- Neural Network: Same concept as knn - use random forest's best output and iterate again with max_features

