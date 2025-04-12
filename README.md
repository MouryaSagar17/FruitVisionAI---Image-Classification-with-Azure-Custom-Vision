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
