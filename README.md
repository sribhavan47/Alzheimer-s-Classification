# Alzheimer's Classification
An end-to-end implementation of Machine Learning.This Python script, along with the associated web application, forms the core of the "Alzheimer's Classification" project. The code serves as an interface for classifying patients as either "non-demented" or "demented" based on a machine learning model's predictions.

Here's a breakdown of the key components and functionalities:

**Importing Libraries:**

```
The code begins by importing the necessary Python libraries. These include numpy for numerical operations, Flask for web application development, and pickle for loading a pre-trained machine learning model.
```
**Initializing the Flask App:**
```
The Flask web application is initialized, and a reference to the pre-trained machine learning model is loaded into memory. This model is stored in a file named 'model_.pkl'.
```
**Default Web Page:**
```
The Flask route '/' is defined as the default page of the web app. When users access the root URL, they are presented with an HTML template (presumably named 'index.html').
```
**Prediction Route:**
```
Another route, '/predict1', is defined. This route handles POST requests, typically triggered by a user clicking a "Predict" button on the web interface.
```
**Making Predictions:**
```
In the predict1 route, the code extracts input features from the HTML form submitted by the user. These features are collected and converted into a format suitable for prediction.
```
**Model Prediction:**
```
The pre-trained machine learning model is used to make predictions based on the input features. The predictions are binary, with '1' representing "non-demented" and '0' representing "demented."
```
**Rendering Results:**
```
The prediction results are rendered back to the HTML template, and the user is informed of whether the patient is classified as "non-demented" or "demented."
```
**Running the Web Application:**
```
The script includes a conditional block that runs the Flask app when executed directly. This allows the web application to run with debugging enabled.
```
## Getting Started
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/Alzheimers-Classification.git
   cd Alzheimer's-Classification
2.Install the required Python packages using pip:
```bash
  import flask
  import gunicorn
  import pandas as pd
  import seaborn as sns
  import matplotlib.pyplot as plt
  import sklearn
  import numpy as np
  import pickle4 as pickle
  import sklearn as sklearn
```
3.Install the required Python packages using pip:

```bash
pip install -r requirements.txt
```
4.Run the Flask web application:
```bash
python app.py
```
5.Access the web application in your web browser at http://localhost:5000.

**Usage:**


When you access the web application, you'll see an input form where you can provide the required patient data for classification.

Fill in the relevant patient information and click the "Predict" button.

The model will make a prediction, and you'll receive the result on the same page, indicating whether the patient is non-demented or demented.

**Contributors**:
- [<img src="https://avatars.githubusercontent.com/u/91361858?v=4" width="40" height="40" alt="GitHub Icon">](https://github.com/SrSurajithPranav)
