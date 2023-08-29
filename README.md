# Next-Day-Rain-Prediction
This repository shows if Sydney would have a rain (or not) tomorrow. I coded 5 predictive algorithms and compared their performances. 

## Source data
The original source is the [Australian Government's Bureau of Meteorology](http://www.bom.gov.au/climate/dwo/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkML0101ENSkillsNetwork20718538-2022-01-01). The .csv file used in this analysis was prepared by the instructors of IBM's course _Machine Learning with Python_. Thanks to Joseph Santarcangelo, Ph.D. and Svitlana Kramar. The file contains observations of weather metrics for each day from 2008 to 2017 in Sydney. The dataset is imbalanced; only 35% of our target's records are positive class (i.e. raining tomorrow). The total number of records is 3,271. 

## Conclusion
Out of the five models analyzed (KNN, Logistic Reg, SVM, Decision Tree, Random Forest) for Sydney's historical weather data, our best models for predicting next-day rain are Logistic Regression ('C' parameter is equal to 10, the rest of the parameters are default) and Random Forest Classifier ('max_feature' parameter is equal to 1, the rest of the parameters are default). The weighted f1-scores for both models are equal to 0.83. 

![image](https://github.com/marvin-rubia/Next-Day-Rain-Prediction/assets/140475770/f00cfc85-72be-4691-86d2-eb9eab30b518)
