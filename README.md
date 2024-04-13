Pretictive Text Analytics For Sentiment analysis on Customer Feedback
This project implements a machine learning model for sentiment analysis on customer feedback. The model is trained on customer feedback data to predict the sentiment (positive or negative) associated with each piece of feedback.

Overview
The project consists of the following components:

Model Training: 
Machine learning models (CNN, Bi-LSTM, GRU, Hybrid CNN) are trained on a dataset of customer feedback to learn patterns and relationships between text data and sentiment labels.

Model Evaluation: 
The trained models are evaluated using a separate test dataset to assess their performance in predicting sentiment accurately.

Model Deployment: The model with the highest accuracy is deployed using AWS Lambda and API Gateway to create an endpoint for making predictions via HTTP requests.

Project Structure
data/: Contains the dataset used for training and testing the models.
models/: Contains trained model files saved using MLflow.
src/: Contains the source code for model training, evaluation, and deployment.
README.md: This file, providing an overview of the project and instructions for usage.
requirements.txt: List of Python dependencies required to run the project.
Usage
Training the Models
To train the machine learning models, follow these steps:

Prepare the dataset:
Ensure that the dataset is preprocessed and split into training and testing sets.
Run the model training script: Execute the appropriate Python script (train_cnn.py, train_lstm.py, etc.) to train the desired model.
Evaluating the Models
To evaluate the trained models, follow these steps:

Run the model evaluation script: Execute the evaluation script (evaluate_model.py) to assess the performance of each model on the test dataset.
Deploying the Model
To deploy the model using AWS Lambda and API Gateway, follow these steps:

Set up AWS credentials: Configure your AWS credentials using the AWS CLI or environment variables.
Package the model: Package the model files and Lambda function handler code into a deployment package.
Create a Lambda function: Create a new Lambda function on AWS using the deployment package.
Set up API Gateway: Create a new API on API Gateway and configure a resource and method to trigger the Lambda function.
Deploy the API: Deploy the API to a stage to obtain an endpoint URL for making predictions.
This project is licensed under Group 4E
