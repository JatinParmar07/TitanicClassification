# TitanicClassification

The Titanic Survival Prediction project aims to predict whether a passenger survived the Titanic disaster using machine learning models. The dataset contains various features like passenger class, sex, age, number of siblings/spouses aboard, and fare. The goal of this project is to create a model that predicts whether a passenger survived (1) or not (0) based on these features.

## Data Preprocessing
#### Data Cleaning and Handling Missing Values
The dataset was preprocessed by filling or removing missing values in critical columns such as age and fare, ensuring the data was ready for model training.

#### Feature Engineering
The relevant features were extracted from the raw data, including converting categorical variables (e.g., Sex) into numerical values for machine learning models to process. Missing values were filled, and continuous features were standardized for better model performance.

## Modeling
#### Train-Test Split
The data was split into training and testing sets to evaluate model performance. A typical split ratio of 85% training and 15% testing was used.

#### Logistic Regression
Initially, a logistic regression model was used to predict passenger survival. Logistic regression was chosen due to its simplicity and effectiveness in binary classification tasks.

#### Ensemble 
Here we used an Ensemble of Logistic Regression, Random Forest and XGB to handle unbalanced data because despite logistic regression giving good accuracy it failed to predict new data. 
Model Evaluation
#### Accuracy
The model's performance was evaluated primarily through accuracy, indicating how many predictions were correct out of the total predictions.

#### Other Metrics
Additional evaluation metrics, including precision, recall, and the F1-score, were used to assess the model's ability to classify survivors and non-survivors more comprehensively.
#### Handling Class Imbalance
The dataset was highly imbalanced, with more survivors than non-survivors. Techniques like class weights were used to mitigate this imbalance and improve model predictions.

## Submission
After training the model, the final predictions were generated for the test dataset. These predictions were stored in a CSV file with the passenger ID and their predicted survival status, which was then prepared for submission to Kaggle.

## Conclusion
The Logistic Regression model achieved a reasonable accuracy, but the eNSEMBLE model showed a much better performance in predicting survival outcomes.
