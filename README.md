# MLflow PySpark Pipeline for Diabetes Prediction using Azure Databricks

This project showcases how to build a machine learning pipeline for predicting diabetes in patients using PySpark and MLflow, and how to deploy it using Azure Databricks.


## Overview

The MLflow PySpark Pipeline for Diabetes Prediction is a comprehensive example of how to use the MLflow library to build a machine learning pipeline to predict diabetes in patients. The pipeline is built using various PySpark libraries, such as Pipeline, PipelineModel, Logistic Regression, BinaryClassificationEvaluator, and MulticlassClassificationEvaluator.

The first step is to set the MLflow experiment for diabetes prediction. The next step is to load the diabetes dataset, which is split into training and test sets using the randomSplit function. The hyperparameters for the logistic regression model are set, and the model is trained using the pipeline function.

The categorical features in the dataset are converted to numeric using StringIndexer, and the features vector is created using VectorAssembler. The logistic regression model is defined, and the pipeline is created using these components. The hyperparameters are logged, and the model is trained.

After training the model, the predictions are made on the test data, and the model is evaluated using BinaryClassificationEvaluator and MulticlassClassificationEvaluator. The evaluation metrics, such as area under the ROC curve and accuracy, are logged using the mlflow.log_metric function.

The model is then logged using the mlflow.spark.log_model function, which saves the model to the MLflow registry. The model is then deployed and used to make predictions on new data.


## Dataset

The dataset used in this project is the [Diabetes Prediction dataset from Kaggle](https://www.kaggle.com/datasets/iammustafatz/diabetes-prediction-dataset), which includes medical and demographic data from patients along with their diabetes status (positive or negative). The features include age, gender, body mass index (BMI), hypertension, heart disease, smoking history, HbA1c level, and blood glucose level.


## Prerequisites

- Azure Databricks account
- Diabetes prediction dataset
- PySpark, MLflow, and Azure Databricks libraries


## Getting Started

1. Clone this repository to your local machine

2. Import the diabetes-prediction.ipynb notebook into Azure Databricks

3. Upload the diabetes prediction dataset to Azure Databricks

4. Set up the MLflow experiment

5. Follow the instructions in the notebook to build and deploy the pipeline


## Conclusion

The MLflow PySpark Pipeline for Diabetes Prediction using Azure Databricks provides a complete example of how to build and deploy a machine learning pipeline using PySpark and MLflow on the Azure platform. This pipeline can be used by healthcare professionals to identify patients who may be at risk of developing diabetes and in developing personalized treatment plans.
