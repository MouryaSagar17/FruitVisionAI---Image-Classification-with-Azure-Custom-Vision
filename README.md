# 🍎🍌🍊 Fruit Image Classification with Azure AI Custom Vision (Python)

This project demonstrates how to train and test an image classification model using the **Azure AI Custom Vision** service. The model is trained to identify images of three fruits: **apple**, **banana**, and **orange**.

## 🚀 Project Overview

This lab-based project uses the **Azure Custom Vision** service to:

- Upload and tag fruit images.
- Train a machine learning model to classify images.
- Evaluate the model's accuracy.
- Test the model using new images.
- Publish the model and use it from a client application.

## 📂 Project Structure

```bash
.
├── LabFiles
│   └── Image Classification
│       ├── training-images
│       │   ├── apple
│       │   ├── banana
│       │   └── orange
│       ├── test-images
│       ├── Python
│       │   ├── train-classifier
│       │   │   ├── .env                # Environment variables for training
│       │   │   └── train-classifier.py # Upload and train model
│       │   └── test-classifier
│       │       ├── .env                # Environment variables for prediction
│       │       └── test-classifier.py  # Predict image labels
```
## 🛠️ Prerequisites
Python 3.7+

Azure Subscription

Azure AI Custom Vision resources (Training and Prediction)

## 🧪 Setup and Installation
Clone the repository

```bash
git clone MouryaSagar17/FruitVisionAI---Image-Classification-with-Azure-Custom-Vision.git
cd image-classification/Python
```

Install required Python packages

```bash
pip install azure-cognitiveservices-vision-customvision==3.1.0
```
Configure Environment Variables

Create a .env file in both train-classifier and test-classifier folders with the following format:
```bash
ENDPOINT=<Your Training or Prediction Endpoint>
TRAINING_KEY=<Your Training Key>
PREDICTION_KEY=<Your Prediction Key>
PROJECT_ID=<Your Project ID>
PUBLISHED_NAME=fruit-classifier
```
## 🏋️‍♀️ Training the Model
Navigate to the training folder and run:

```bash
cd train-classifier
python train-classifier.py
```
This script will:

Connect to Azure Custom Vision Training resource

Upload training images from training-images/

Assign tags (apple, banana, orange)

Train the model

## 🔍 Testing the Model
Navigate to the test folder and run:
```bash
cd ../test-classifier
python test-classifier.py
```

This will:

Use the prediction resource

Send test images from test-images/

Output the predicted tag and confidence score

## 📊 Sample Output
apple.jpg: Predicted - apple (95.34%)
banana.jpg: Predicted - banana (92.21%)
orange.jpg: Predicted - orange (93.18%)
## 📘 References
Azure AI Custom Vision

Azure SDK for Python - Custom Vision
