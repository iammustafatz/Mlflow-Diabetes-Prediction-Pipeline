# Mlflow Pyspark Pipeline for Diabetes Prediction

This project demonstrates how to build a machine learning pipeline to predict diabetes in patients using PySpark and MLflow. The pipeline includes preprocessing of the data, training and evaluation of the logistic regression model, and logging the model to the MLflow registry for later use.

Dataset
The dataset used in this project is the Diabetes Prediction dataset from Kaggle, which includes medical and demographic data from patients along with their diabetes status (positive or negative). The features include age, gender, body mass index (BMI), hypertension, heart disease, smoking history, HbA1c level, and blood glucose level.

Requirements
To run this project, you need the following libraries installed:

PySpark
MLflow
Pandas
NumPy
Usage
Clone the repository to your local machine.
Set up your PySpark environment, if not already done.
Run the diabetes_prediction.py file to build and evaluate the machine learning pipeline. The script will automatically log the model and evaluation metrics to MLflow.
To view the logged information, open MLflow UI by running mlflow ui in the terminal and navigating to localhost:5000 in your web browser.
License
This project is licensed under the MIT License.

Credits
The original dataset is available on Kaggle and was provided by the National Institute of Diabetes and Digestive and Kidney Diseases. The code and documentation in this project were created by [Your Name Here].
