# Machine-Learning-Adult-Income-Project-Portfolio
Predicting adult's income with Census information from 1994

# Features: 
Age, workclass, education/number of years of education(I will only use one of the columns since they are a bit repetitive and can make education too much of an impact on the result), marital status/relationship, occupation, race, sex, capital gains, capital loss, hours per week

# Model: 
Logistic regression &  K nearest neighbor
# Data Preprocessing Techniques: 
Handle missing data either by imputing them (using mean, median, or other statistical methods) or removing rows/columns with missing values.
Remove or add a column with the winsorized version of the original column for handling outliers
One-hot coding for converting categorical variables into binary vectors

# Evaluation metric: 
The Receiver Operator Characteristic (ROC) curve (ROC AUC) would be appropriate for my model since my problem is a binary classification problem.

# Plan: 
## Data Preprocessing:
Handle missing data using appropriate techniques like imputing missing values using the mean or median
Winsorize columns
Convert categorical variables (workclass, marital status, occupation, relationship, race, sex) into binary vectors using one-hot encoding.
## Data Splitting:
Split the preprocessed data into training, validation, and test sets. 
## Model Training:
Train a Logistic Regression and a  K nearest neighbor model on the training set using the selected features 
## Model Validation and Performance Analysis:
Evaluate both models on the validation set using the Receiver Operating Characteristic (ROC) curve and calculate the Area Under the ROC Curve (ROC AUC) as the evaluation metric.
## Model Selection:
Choose the model with the higher ROC AUC on the validation set, as it indicates better performance for the binary classification problem.
## Model Improvement 
Fine-tune hyperparameters of the models using techniques like Grid Search to find the optimal combination of hyperparameters that improves ROC AUC.
## Evaluation:
After improving the models, evaluate them on the test set using the ROC curve and ROC AUC.

