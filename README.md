# Diabetes-Prediction-Model
A diabetes prediction model is a machine learning system designed to predict whether an individual has diabetes based on a set of input features. These features typically include medical and demographic information such as blood glucose levels, blood pressure, age, BMI, and other relevant parameters. 
Key Objectives
Implement a K-Nearest Neighbors (KNN) and Random Forest algorithm to classify whether a patient has diabetes.
Use Python and its libraries for data preprocessing, model training, and evaluation.
Compare the performance of both models based on accuracy, precision, recall, and F1-score.
Build an easy-to-understand, maintainable codebase for future improvements.

Dataset
The Pima Indians Diabetes Database consists of the following attributes:

Pregnancies: Number of times the patient has been pregnant
Glucose: Plasma glucose concentration
BloodPressure: Diastolic blood pressure (mm Hg)
SkinThickness: Triceps skinfold thickness (mm)
Insulin: 2-Hour serum insulin (mu U/ml)
BMI: Body mass index (weight in kg/(height in m)^2)
DiabetesPedigreeFunction: Diabetes pedigree function
Age: Age (years)
Outcome: Class variable (0 or 1), where 1 denotes diabetes and 0 denotes no diabetes


Data Preprocessing
Data preprocessing is a crucial step in any machine learning project. In this stage, we handle missing values, normalize data, and split the dataset into training and test sets.

Handling Missing Values
The dataset has some missing or zero values in certain columns such as Glucose, BloodPressure, SkinThickness, Insulin, and BMI. These zero values are not valid and need to be replaced with the median or mean values.

Data Normalization
Next, we normalize the data to ensure that each feature contributes equally to the model’s performance. Standardization rescales features to have a mean of zero and a standard deviation of one.

Splitting the Dataset
We split the dataset into training and testing sets, with 80% of the data used for training and 20% for testing.

Model 1: K-Nearest Neighbors (KNN)
The K-Nearest Neighbors (KNN) algorithm is a simple, yet powerful, classification algorithm. It works by finding the ‘k’ closest points in the training dataset to a given test point and classifying the test point based on the majority class of these neighbors.

Model 2: Random Forest
Random Forest is an ensemble learning method that uses multiple decision trees to classify data. Each tree is trained on a different subset of the dataset, and the final classification is made by averaging the results of all the trees.

Results and Conclusion
After evaluating both models, we compare their performance based on the chosen metrics. In many cases, Random Forest tends to perform better than KNN due to its ensemble nature and ability to handle feature importance.

KNN Accuracy: ~70-75%
Random Forest Accuracy: ~80-85%
The Random Forest algorithm is likely to be the final choice due to its higher accuracy and robustness. However, KNN is simpler and works well for small datasets.
