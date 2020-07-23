Using deep feedforward neural networks to predict 30-day hospital readmission in diabetic patients

Introduction to the Project:

Deep neural networks will be used and evaluated as binary classifiers to predict whether a patient will be readmitted to hospital within 30 days based on pre-discharge factors such as demographics, diagnoses, change in diabetic medications, and reason for discharge. Three traditional classifiers will be used for comparison as well: random forest, k-nearest neighbours, and logistic regression. The best-performing model will also be used to identify risk factors that have the largest impact on readmission. Predicting at the point of hospital discharge whether a patient will be readmitted can allow for allocation of resources to these high risk individuals to reduce readmissions. Additionally, identifying pre-discharge risk factors with the largest impact on readmissions may highlight opportunities for targeted interventions.


Running the Code:

Cleaning and Exploratory Analysis: In order to run the code, download Coding for Cleaning and Exploratory Analysis.Rmd and Dataset_Raw.csv from this repository. Open the Rmd file in RStudio. In the second chunk of code (entitled "Import"), add in the file path for Dataset_Raw.csv on your computer so that it may be saved into the db.raw object. All code may be run in order after this is completed.

Modeling and Evaluation: In order to run this code, download Coding for Modeling and Evaluation.Rmd and Dataset_Modeling.csv from this repository. Open the Rmd file in RStudio. If you do not already have TensorFlow installed, delete the hashtag in front of "#install_tensorflow()" in the first chunk, and then run the first chunk. Otherwise, leave the hashtag in and then run the first chunk. In the second chunk, add in the file path for Dataset_Modeling.csv on your computer so that it may be saved into the db.model object. All code may be run in order after these steps are completed.


File Descriptions:

Coding for Cleaning and Exploratory Analysis.Rmd
- Coding file 1: Rmd file containing code for importing the raw dataset, removing out of scope cases, cleaning, exploratory analysis, and transformation of data prior to modeling.

Coding for Modeling and Evaluation.Rmd
- Coding file 2: Rmd file containing code for creating folds in data, oversampling to balance the class attribute, all modeling, evaluation of modeling performance, and identification of variable importance.

Dataset_Raw.csv
- Raw dataset, prior to any changes being made. The dataset is also available from the UCI Machine Learning Repository (https://archive.ics.uci.edu/ml/datasets/Diabetes+130-US+hospitals+for+years+1999-2008)

Dataset_Exploration.csv
- Dataset used for exploration. Out of scope cases, variables with large numbers of missing values, and variables with low variance have been removed. Certain categories of categorical variables have been condensed.

Dataset_Modeling.csv
- Dataset ready for modeling. All variables from the exploration dataset have been transformed to contain numeric values between 0 and 1. Creation of folds and oversampling has not yet been completed.

id_mapping.csv
- Document that originally came with the raw dataset containing the names of each level for three variables: Admission Source ID, Discharge Disposition ID, and Admission Type ID.

Project Report.pdf
- Report on Project findings; includes introduction, literature review, data description and exploration, overall approach, results, and conclusion of findings

Results for Cleaning and Exploratory Analysis.html
- html document knitted from Coding for Cleaning and Exploratory Analysis.Rmd to show the results of the code.

Results for Modeling and Evaluation.html
- html document knitted from Coding for Modeling and Evaluation.Rmd to show the results of the code.

