# CST2101-W23-Project-FINAL_PROJECT_KARANDEEP_041042181

OVERVIEW:
Analyzing diabetic data and addressing some significant business issues/questions are the goals of this initiative.

AIM:
The goal of the project is focused on Exploratory Data Analysis and Model Training using Python.

PROBLEM STATEMENT:

One of the most prevalent diseases in the world, diabetes has an increasing prevalence throughout time. Although the primary cause of diabetes is still unknown, scientists think that both hereditary and environmental lifestyle factors play a significant influence in the disease.

Research on the Pima tribe, an American tribe, was conducted a few years ago (also known as the Pima Indians). It was discovered that the women of this tribe get diabetes quite early. These instances were chosen from a bigger database under a number of restrictions. In specifically, all patients were Pima Native women who were at least 21 years old. Here, we are performing exploratory data analysis and developing a classification model to analyse several facets of diabetes in the Pima Indian tribe.

DATASET INFORMATION:

Below is the attribute information:

Pregnancies: Number of times pregnant
Glucose: Plasma glucose concentration a 2 hours in an oral glucose tolerance test
Blood pressure: Diastolic blood pressure (mm Hg)
SkinThickness: Triceps skinfold thickness (mm)
Insulin: 2-Hour serum insulin (mu U/ml) test
BMI: Body mass index (weight in kg/(height in m)^2)
DiabetesPedigreeFunction: A function that scores likelihood of diabetes based on family history
Age: Age in years
Outcome: Class variable (0: the person is not diabetic or 1: the person is diabetic)

Here, are some Quick Insights for the work done:

EXPLORATORY DATA ANALYSIS:

1. There are 1000 Records and 9 Features.
2. Size of dataset= 9000
3. There are No Null Values.
4.  The majority of persons have blood pressures between (60 and 80) mm Hg. The BloodPressure distribution appears to be normal as well.
    Moreover, there is a slight bit of skewness to the right, indicating the possibility of outliers in the dataset that need to be examined.
    Also, there is a second bump at 0 mm Hg, indicating some data inaccuracy since 0 blood pressure is not conceivable biologically.
5. The BMI for the person having the highest glucose is 42.9
6. From correlation matrix it is observed that: 
'Age' and the 'Pregnancies' are the two features having positive correlation.

'SkinThickness' and 'Insulin' also presented positive correlation.

'SkinThickness' and'BMI' also has positive correlation.

However, these correlations are not so strong enough hence, No multi-collinearity is exhibited here.

STANDARDISATION AND DATA SPLITTING: 

First data is standardised to rescale all the features in a particular range using the StandardScaler() and further, data is splitted with keeping test data size as 0.15 and rest as training data and also, the stratified sampling technique is employed to make sure that all the samples are included from the each strata(subgroup).

MODELLING:

 Two models are employed: A. LOGISTIC REGRESSION 
                          B. RANDOM FOREST
RESULTS AND ANALYSIS:

Random Forest has higher accuracy on both train and test dataset.

Also,the Recall scores also high in case of Random forest when compared with the Logistic Regression.

F1 scores for RandomForest model is also higher.
However, the Precision scores are slightly higher for the Logistic regression.

Overall, it can be concluded that the RandomForest Performed better.
