# Next-Day-Rain-Prediction
This repository shows if Sydney would have a rain (or not) tomorrow. I coded 5 predictive algorithms and compared their performances. 

## Source data
The original source is the [Australian Government's Bureau of Meteorology](http://www.bom.gov.au/climate/dwo/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkML0101ENSkillsNetwork20718538-2022-01-01). The .csv file used in this analysis was prepared by the instructors of IBM's course _Machine Learning with Python_. Thanks to Joseph Santarcangelo, Ph.D. and Svitlana Kramar. The file contains observations of weather metrics for each day from 2008 to 2017 in Sydney. The dataset is imbalanced; only 35% of our target's records are positive class (i.e. raining tomorrow). The total number of records is 3,271. 

## Conclusion
![image](https://github.com/marvin-rubia/Next-Day-Rain-Prediction/assets/140475770/159f4e97-f4b8-4f52-87ab-5405866841e5)

NOTE: LR and SVM are tied using our primary metrics. But in terms of ROC-AUC score, LR (with 0.866) slightly beats SVM (with 0.860). 

Out of the five models developed for Sydney's historical weather data from 2008 to 2017, our best model for predicting next-day rain is **Logistic Regression** (C=0.1, solver='liblinear', the rest of the parameters are default). Its weighted f1-score is 0.830, its weighted recall is 0.840, and its ROC-AUC score is 0.866. Decision Tree (max_depth=3, the rest of the parameters are default) performed the weakest. 

Weather forecasts are accompanied by probability and our logistic regression model can readily give the probability of rain tomorrow using the `.predict_proba()` method from Sci-kit Learn. 

## How to see my work?
Check the uploaded [Notebook](https://github.com/marvin-rubia/Next-Day-Rain-Prediction/blob/main/Next_Day_Rain_Prediction.ipynb) in this repository. 
