# Crop Recommendation System

This project is a Machine Learning-based Crop Recommendation System that helps farmers decide which crop to plant based on soil nutrients and environmental conditions. The project uses a Support Vector Machine (SVM) for the prediction and is deployed using Flask.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Model](#model)
- [Web Application](#web-application)
- [Contributing](#contributing)
- [License](#license)

## Introduction
The Crop Recommendation System aims to assist farmers in choosing the right crop for their land by analyzing various factors like soil nutrients and environmental conditions. By providing these inputs, the system predicts the most suitable crop to maximize yield.

## Features
- Predicts the best crop to plant based on input conditions.
- Uses Support Vector Machine (SVM) for high accuracy.
- Simple and user-friendly web interface built with Flask.
- Easy to extend and customize.

## Installation
Follow these steps to get the project up and running on your local machine.

### Prerequisites
- Python 3.7+
- Flask
- scikit-learn
- pandas
- numpy

### Steps
1. Clone the repository
    ```bash
    git clone https://github.com/yourusername/crop-recommendation-system.git
    cd crop-recommendation-system
    ```

2. Create a virtual environment
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. Install the required packages
    ```bash
    pip install -r requirements.txt
    ```

4. Run the Flask application
    ```bash
    python app.py
    ```

5. Open your web browser and go to `http://127.0.0.1:5000/`.

## Usage
1. Open the web application in your browser.
2. Enter the required input parameters: Nitrogen (N), Phosphorus (P), Potassium (K), pH, Rainfall, Humidity, and Temperature.
3. Click the "Predict" button to get the recommended crop.

## Dataset
The dataset used for training the model includes various features such as:
- Nitrogen (N)
- Phosphorus (P)
- Potassium (K)
- pH
- Rainfall
- Humidity
- Temperature

You can find the dataset in the `data` directory.

## Model
The model is built using a Support Vector Machine (SVM) classifier. The training script is available in the `model` directory. To retrain the model, you can run the training script as follows:

```bash
python model/train_model.py
