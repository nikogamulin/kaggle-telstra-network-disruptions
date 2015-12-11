#Telstra Recruiting: Network Disruptions

#Predict service faults on Australia's largest telecommunications network

The goal of the problem is to predict Telstra network's fault severity at a time at a particular location based on the log data available. Each row in the main dataset (train.csv, test.csv) represents a location and a time point. They are identified by the "id" column, which is the key "id" used in other data files. 

Fault severity has 3 categories: 0,1,2 (0 meaning no fault, 1 meaning only a few, and 2 meaning many). 

Different types of features are extracted from log files and other sources: event_type.csv, log_feature.csv, resource_type.csv, severity_type.csv. 

Note: “severity_type” is a feature extracted from the log files (in severity_type.csv). Often this is a severity type of a warning message coming from the log. "severity_type" is categorical. It does not have an ordering. “fault_severity” is a measurement of actual reported faults from users of the network and is the target variable (in train.csv).

##File descriptions (data)
* train.csv - the training set for fault severity
* test.csv - the test set for fault severity
* sample_submission.csv - a sample submission file in the correct format
* event_type.csv - event type related to the main dataset
* log_feature.csv - features extracted from log files
* resource_type.csv - type of resource related to the main dataset
* severity_type.csv -  severity type of a warning message coming from the log


##Project files
* [data_explorer.ipynb - exploratory data analysis of the data provided for the competition with a simple neural network at the end](https://github.com/nikogamulin/kaggle-telstra-network-disruptions/blob/master/data_explorer.ipynb)

##References
* [Predict service faults on Australia's largest telecommunications network](https://www.kaggle.com/c/telstra-recruiting-network)
* [t-SNE](https://lvdmaaten.github.io/tsne/)
* [Keras (Python Deep Learning Library)](https://github.com/fchollet/keras)

