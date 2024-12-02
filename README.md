# MLPrediction
The highest internet users, namely the age group included in Generation Z (Gen Z), utilize their use to follow influencers on social media which can cause a trend in various circles. The development of these trends causes consumptive behavior for its followers. Students as part of Gen Z who are dominated by those whose source of income is from parents have different consumptive levels in following trends to fulfill the lifestyle in the surrounding environment. The lifestyle followed depends on the socioeconomic status (SES) category assessed by the cost of regular monthly expenses. Therefore, in this research, machine learning techniques, namely supervised learning predict the lifestyle of students by learning the features used and classifying based on the class, namely SES. Prediction with the CatBoost algorithm is used to determine the level of prediction accuracy and influencing factors based on the input data given.

#**Method**
**A.	Research Approach**
This research uses quantitative research methods. The analysis model uses CatBoost and is contained in performance metrics consisting of 5 parts, namely confusion matrix, accuracy, precision & recall, f1 score, and area under ROC curve (AUC). Information collection is done with SES data of UIN Jakarta students obtained through online questionnaire distribution.  

**B.	Research Population and Sample**
The research sample is part of the population taken as a data source and represents the entire population. In this study, the sample will be taken from the total population of UIN Jakarta students in the 2019-2022 batch who fall into the Gen Z age category with a total of 25,607 students obtained from the UIN Jakarta Information Technology and Database Center (Pustipanda). The sample used in this study is by using the proportionate stratified random sampling method and the sample size in this study is determined using the Slovin formula with an error tolerance limit of 5%. The sample that became respondents in the study was 394 people who were rounded up by researchers to 400 students from active UIN Jakarta class of 2019-2022.  

**C.	Data Pre-Processing**
In the initial stage, data pre-processing is carried out to clean the data and make it suitable for the machine learning model created and can improve the accuracy and efficiency of the machine learning model. Data pre-processing consists of several stages, namely, obtaining data sets, importing libraries, importing data sets, finding missing data, coding categorical data, separating datasets into 80% training and 20% testing sets, and feature scaling.

**D.	Processing**
Machine learning model training is the process where the CatBoost algorithm is given training data that it can learn from. Model training works to adjust the best weights and biases to the algorithm to minimize the loss function over the prediction range. The loss function determines how to optimize the machine learning algorithm. 

**E.	Evaluation Metrics**
After training the model, it can evaluate its performance on testing data and can see what features are most influential by representing them in performance metrics including confusion matrix, accuracy, precision & recall, f1 score, and area under roc curve (AUC).  

#**Result**
**A.	CatBoost Modeling Results**
  The resulting "Best Test" value of the CatBoost modeling is 0.7495. The "Best Test" value indicates the best performance achieved by the CatBoost model on certain evaluation metrics during the training process. The evaluation metrics consist of accuracy, F1-score, precision & recall, confusion matrix, and AUC. 
The results of the "Best Iteration" value of the CatBoost modeling created show the iterations or rounds during training with the best performance at the 188th iteration. In gradient boosting, the algorithm iteratively adds weak testing data (usually decision trees) to the model, with each new testing data to correct previous errors.  
 
![image](https://github.com/user-attachments/assets/fafec1dd-3d3a-4642-b42f-2488ed10f007)

**B.	Feature Importances**
Determining the accuracy of SES using CatBoost modeling requires features selected from the collected data. In this CatBoost modeling, 14 features were selected.   In this study, the level of importance of features is divided by rank into levels of importance based on a range of scores or percentiles with four levels of importance, namely very high, high, medium, and low [27]. The feature boundaries of each level have different proportions, among others, scores in the top 10% are very high, features in the top 25% are high, features in the top 50% are medium, and the rest are low [28]. The tuition class, occupation, parents, and entertainment expenditure are the 4 highest features in importance out of 14 features used in CatBoost modeling based on the correlation results of the feature matrix with the target label, SES score. 

**C.	Accuracy**
The accuracy results of SES using CatBoost modeling obtained an accuracy value from the training data results of 0.8625 which explains that the CatBoost classifier can predict the class label correctly by 85.94% of the input data.  

**D.	Precision, Recall, & F1 Score**
The following are the results of the CatBoost modeling training data in the precision, recall, and F1-score matrices contained.
<img width="181" alt="{107C7E8E-8F3E-46C9-B49D-3C9979350B9F}" src="https://github.com/user-attachments/assets/fb5fb50b-2762-4ada-b12a-664e91992ab3">
Precision is when the model predicts a data sample from each class and the result shows the proportion of positive predictions or the condition that the prediction result is correct and the reality is correct (TP). The recall is based on all data instances that are actually positive or belong to each class that correctly predicts a positive prediction out of the total positives. The F1-score is the harmonic mean of precision and recall by combining both measures into one score or F1-score for each class. Support is the number of examples in the data set that belong to each class. 

**E.	Confusion Matrix**
Interpreting model performance using a confusion matrix in understanding how well the model performs and can help improve model performance by combining several metrics that can be calculated including accuracy, precision & recall, and F1-score. The confusion matrix of the CatBoost modeling performed results in predicted and real conditions described in TP, FP, TN, and FN consisting of four classes as follows:
![image](https://github.com/user-attachments/assets/4cb4ad76-2cd2-48e4-8ed4-7adaf0c0bc3d)

**F.	Area Under ROC Curve (AUC)**
Area Under ROC Curve (AUC) in Figure 4. shows the results of CatBoost modeling as part of the model performance evaluation metric used based on the class contained in the overall data, which is divided into 4 classes that have a very good classification with a value above 0.90 in each class.
![image](https://github.com/user-attachments/assets/93165e7d-3c60-466e-aff0-10b1f64a887a)
Based on the prediction results of the lifestyle of UIN Jakarta students according to their SES category, using the CatBoost algorithm, it is known that the UKT class greatly determines the lifestyle of each UIN Jakarta student based on the level of each student's SES category. This can also prove that the UKT class obtained by each UIN Jakarta student is in accordance with their economic capabilities.  
Social class which is an external factor of this lifestyle is influenced by the economic level and consumption patterns of UIN Jakarta students according to their respective SES levels. This statement is also supported by [24] who revealed that consumption patterns and choices in using their time and money affect their lifestyle. Therefore, the results of this study can be used as financial literacy material for UIN Jakarta students to better manage their expenses by minimizing the purchase of products that do not meet their needs by prioritizing the desire to follow trends.  
In addition, marketers in the environment around UIN Jakarta can adjust products based on the personalization of UIN Jakarta students according to the economic level of the desired target market. The results of this study are also in line with the results of research [8] which states that the cost of household consumption expenditure to meet the needs of life has shifted 

#**Conclusion and Recommedation**

