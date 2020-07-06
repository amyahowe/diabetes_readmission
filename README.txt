Using deep feedforward neural networks to predict 30-day hospital readmission in diabetic patients

Introduction to the Project:

Deep neural networks will be used and evaluated as binary classifiers to predict whether a patient will be readmitted to hospital within 30 days based on pre-discharge factors such as demographics, diagnoses, change in diabetic medications, and reason for discharge. The best-performing model will also be used to identify risk factors that have the largest impact on readmission. Predicting at the point of hospital discharge whether a patient will be readmitted can allow for allocation of resources to these high risk individuals to reduce readmissions. Additionally, identifying pre-discharge risk factors with the largest impact on readmissions may highlight opportunities for targeted interventions.

The project is not yet complete. So far, the data cleaning, exploratory analysis, and transformation prior to modelling is complete.


Running the Code:

In order to run the code, download Coding for Cleaning and Exploratory Analysis.Rmd and Dataset_Raw.csv from this repository. Open the Rmd file in RStudio. In the second chunk of code (entitled "Import"), add in the file path for Dataset_Raw.csv on your computer so that it may be saved into the db.raw object. All code may be run in order after this is completed.


File Descriptions:

Coding for Cleaning and Exploratory Analysis.Rmd
- Rmd file containing all code so far, including importing the raw dataset, removing out of scope cases, cleaning, exploratory analysis, and transformation of data prior to modeling.

Dataset_Raw.csv
- Raw dataset, prior to any changes being made. The dataset is also available from the UCI Machine Learning Repository (https://archive.ics.uci.edu/ml/datasets/Diabetes+130-US+hospitals+for+years+1999-2008)

Dataset_Exploration.csv
- Dataset used for exploration. Out of scope cases, variables with large numbers of missing values, and variables with low variance have been removed. Certain categories of categorical variables have been condensed.

Dataset_Modeling.csv
- Dataset ready for modeling. All variables from the exploration dataset have been transformed to contain numeric values between 0 and 1.

id_mapping.csv
- Document that originally came with the raw dataset containing the names of each level for three variables: Admission Source ID, Discharge Disposition ID, and Admission Type ID.

Project Report - Lit Review, Data Description and Approach.pdf
- Report on Project findings; currently includes the Introduction, Literature Review, Data Description and Exploration as well as the Approach.

Results for Cleaning and Exploratory Analysis.html
- html document knitted from Coding for Cleaning and Exploratory Analysis.Rmd to show the results of the code

