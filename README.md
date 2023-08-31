# Next-Day-Rain-Prediction
This repository shows if Sydney would have a rain (or not) tomorrow. I coded 5 predictive algorithms and compared their performances. 

## Source data
The original source is the [Australian Government's Bureau of Meteorology](http://www.bom.gov.au/climate/dwo/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkML0101ENSkillsNetwork20718538-2022-01-01). The .csv file used in this analysis was prepared by the instructors of IBM's course _Machine Learning with Python_. Thanks to Joseph Santarcangelo, Ph.D. and Svitlana Kramar. The file contains observations of weather metrics for each day from 2008 to 2017 in Sydney. The dataset is imbalanced; only 35% of our target's records are positive class (i.e. raining tomorrow). The total number of records is 3,271. 

## Conclusion
![image](https://github.com/marvin-rubia/Next-Day-Rain-Prediction/assets/140475770/f2abf2b6-5df7-43f4-bcfe-323cd7ec6a9b)

Out of the five models analyzed for Sydney’s historical weather data from 2008 to 2017, our best model for predicting next-day rain is __Logistic Regression__ (C=0.1, solver=‘liblinear’, the rest of the parameters are default). Its weighted f1-score is 0.83. __Decision Tree__ (max_depth=4, the rest of the parameters are default) performed the weakest prediction with a score of 0.77.

## I wrote a blog about this
I wrote an educational blog that guides a reader from source data to the conclusion here: [Will it Rain Tomorrow? Prediction using 5 Machine Learning Algorithms](https://marvinrubia.medium.com/will-it-rain-tomorrow-prediction-using-5-machine-learning-algorithms-4eb069952ce5). It has additional comments about my thinking process that are not found in my Jupyter Notebook.
