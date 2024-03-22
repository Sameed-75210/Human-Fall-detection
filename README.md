# Human Fall Detection using Smartphone Sensors

## Overview
This project aims to develop a system for detecting human falls using data collected from smartphone sensors. Falls pose a significant risk, especially for the elderly or individuals with mobility issues. By leveraging data from sensors commonly found in smartphones, such as accelerometers and gyroscopes, we can create a system capable of automatically detecting falls and alerting caregivers or emergency services.

## Introduction
Falls are a leading cause of injury and mortality, especially among older adults. Quick detection and response to falls can significantly improve outcomes and reduce the risk of complications. In this project, we explore the feasibility of using smartphone sensors to detect falls in real time.

## Dataset
The dataset used in this project contains data collected from various sensors embedded in smartphones. It includes accelerometer and gyroscope readings from different body locations, such as the ankle, pocket, belt, neck, and wrist. Additionally, the dataset provides information about the activity being performed during each recording, such as walking, standing, sitting, lying, or falling.

## Data Preprocessing
The dataset underwent several preprocessing steps, including:

1) Handling missing values: Missing values were imputed using median values for the respective columns.
2) Feature engineering: Additional features were derived from the raw sensor data to enhance model performance.
3) Data normalization: Sensor readings were standardized to have zero mean and unit variance.

## Exploratory Data Analysis (EDA)
EDA was performed to gain insights into the distribution of activities and sensor readings. Visualizations such as histograms, scatter plots, and count plots were used to explore the data and identify patterns.

## Model Development
Several machine learning models were trained and evaluated for fall detection using the preprocessed dataset. The models include:
- **Random Forest Classifier**
- **Logistic Regression**
- **Support Vector Machine (SVM)**

For each model, the dataset was split into training and testing sets. Grid search with cross-validation was employed to tune hyperparameters and optimize model performance.

### Model Evaluation
The models were evaluated based on accuracy scores and classification reports. The best-performing model was selected for further analysis.

## Results
The results of the model evaluation are summarized as follows:

- **Random Forest Classifier** achieved an accuracy of 99.98% on the test set.
- **Logistic Regression** achieved an accuracy of 96.27% on the test set.
- **Support Vector Machine (SVM)** achieved an accuracy of 99.87% on the test set.

Based on these results, the Random Forest Classifier was chosen as the final model due to its superior performance.

## Model Deployment

The trained Random Forest Classifier model was saved for future use. Deployment of the model can be done in various environments, including mobile applications for real-time fall detection.


