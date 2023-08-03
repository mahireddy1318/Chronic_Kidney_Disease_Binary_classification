Chronic_Kidney_Disease


AIM : is to check the person has Chronic_Kidney_Disease or Not, using Past kidney disease patients records with Machine Leaning Techniques.
 
In this document i'm going to explain how i solved chronic_kidney_disease project. This is a Binary classification project.

for this i used chronic_kidney_disease.csv dataset from kaggale also avalible on UCI.

Initially i gone throw data set and absorving relationship(description of data) between data and Identified missing some data points.
After that I used to preprocessed the data as following

1. Data cleaning
2. EDA
3. Missing value tratment using random sampling
4. Label Encoding

Now our cleaned dataset is ready for Modeling

5. Model Building

using train_test_split method we divided Train and Test data.

Now i fit the data with all classifiers and did hyper perameter tuning using GridSearch CV

6. Obtained model performace using accuracy score, confusion matrix, classification report.

At last i compared all model and get to know which model gives good accuracy.

Here is the comparision among all models...


Models	Test Scores
2	RandomForestClassifier	1.0000
4	GradientBoostingClassifier	0.9875
5	XGBClassifier	0.9875
7	ExtraTreesClassifier	0.9875
3	AdaBoostClassifier	0.9750
6	CatBoostClassifier	0.9750
8	LGBMClassifier	0.9750
1	DecisionTreeClassifier	0.9375
0	KNeighborsClassifier	0.6500