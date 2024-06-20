# Heart_Disease_Prediction
## Introduction
This project predicts the presence of heart disease based on various health metrics using logistic regression. The aim is to aid in early detection and prevention efforts.

## Dataset
The dataset used is the Heart Disease dataset from Kaggle, which includes features such as age, sex, chest pain type, resting blood pressure, serum cholesterol, and more.

## Getting Started
### Running on Google Colab
1. Open Google Colab.
2. Create a new notebook.
3. Upload the dataset (heart_disease_data.csv) to the Colab environment.                       
### Data Preparation and Model Training
#### Data Loading and Splitting                                                                
 1. Load Dataset: Load the heart disease dataset (heart_disease_data.csv) using Pandas. This dataset contains columns representing different health metrics (features) and a target variable indicating the presence or absence of heart disease.

 2. Split Features and Target: Separate the dataset into features (X) and the target variable (Y). Features include age, sex, chest pain type, resting blood pressure, serum cholesterol, etc. The target variable (Y) indicates whether a person has heart disease (1) or not (0).

#### Data Splitting for Training and Testing
Train-Test Split: Split the dataset into training and testing sets using train_test_split from sklearn.model_selection. This ensures that the model is trained on a portion of the data and tested on another unseen portion to evaluate its performance.
### Model Training
#### Logistic Regression Model
 1. Model Initialization: Initialize a logistic regression model using LogisticRegression() from sklearn.linear_model.

 2. Model Training: Fit the logistic regression model to the training data (X_train and Y_train). This step involves learning the relationship between the input features and the target variable using the training dataset.

### Model Evaluation
#### Accuracy Metrics
 1. Training Accuracy: Calculate the accuracy of the model on the training data (X_train and Y_train) using accuracy_score from sklearn.metrics. Training accuracy shows how well the model predicts the target variable on data it has seen during training.

 2. Testing Accuracy: Calculate the accuracy of the model on the testing data (X_test and Y_test) using accuracy_score. Testing accuracy evaluates how well the model generalizes to new, unseen data.

### Prediction Example
#### Making Predictions
 1. Input Data: Prepare example input data (e.g., age, sex, chest pain type, etc.) to predict whether a person has heart disease.
    -> Age: The age of the individual.
                                                           
    -> Sex: The gender of the individual (1 = male, 0 = female).
    
    -> ChestPainType: The type of chest pain experienced by the individual (e.g., typical angina, atypical angina).
    
    -> RestingBloodPressure: The resting blood pressure of the individual (in mm Hg).
    
    -> Cholesterol: The cholesterol level of the individual (in mg/dL).
    
    -> FastingBloodSugar: Indicates whether the fasting blood sugar level is greater than 120 mg/dL (1 = yes, 0 = no).
    
    -> RestingECG: The resting electrocardiographic results (e.g., normal, abnormal).
    
    -> MaxHeartRate: The maximum heart rate achieved during exercise.
    
    -> ExerciseInducedAngina: Indicates whether exercise induced angina (1 = yes, 0 = no).
    
    -> STDepression: The ST depression induced by exercise relative to rest.
    
    -> STSegment: The slope of the peak exercise ST segment.
    
    -> NumMajorVessels: The number of major vessels (0-3) colored by fluoroscopy.
    
    -> Thalassemia: A blood disorder affecting the production of hemoglobin.
    
    -> Target: The presence of heart disease (1 = heart disease present, 0 = heart disease not present)

 3. Prediction: Use the trained logistic regression model to predict whether the input data indicates the presence or absence of heart disease.

#### Interpretation of Results
Prediction Interpretation: Based on the prediction output (0 or 1), interpret whether the model predicts that the person has heart disease or not.
### Results
Accuracy Metrics: Display the training and testing accuracies of the logistic regression model. These metrics provide insights into how well the model performs in predicting heart disease based on the dataset features.
