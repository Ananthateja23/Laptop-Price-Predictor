# Laptop Price Predictor

This project predicts laptop prices based on user-input specifications using machine learning techniques.
It employs a regression model trained on a dataset of various laptop features to estimate the price of a laptop given its specifications.

## Table of Contents

* [About](#about)
* [Features](#features)
* [Dataset](#dataset)
* [Model Training](#model-training)
* [Files](#files)
* [Installation](#installation)
* [Usage](#usage)
* [Deployment](#deployment)


## About

The Laptop Price Predictor is a machine learning application that estimates the price of a laptop based on its specifications.
It utilizes a regression model trained on a dataset containing various laptop features to make accurate price predictions.

## Features

* **User Input Interface**: Allows users to input laptop specifications and receive an estimated price.
* **Machine Learning Model**: Utilizes a regression model trained on a comprehensive dataset of laptop features.
* **Data Preprocessing**: Includes steps for cleaning and preparing data for model training.
* **Model Evaluation**: Assesses model performance using metrics like R² score and Mean Absolute Error.

## Dataset

The model is trained on a dataset containing various laptop specifications and their corresponding prices.
The dataset includes features such as brand, processor type, RAM size, storage capacity, and more.

## Model Training

The model is trained using a regression algorithm.
The training process involves the following steps:

1. **Data Preprocessing**: Cleaning and preparing the dataset for training.
2. **Feature Selection**: Identifying the most relevant features for predicting laptop prices.
3. **Model Training**: Training the regression model on the prepared dataset.
4. **Model Evaluation**: Assessing the model's performance using appropriate metrics.

## Files

* `app.py`: The main application file that runs the Streamlit app.
* `Laptop-Price-predictor.ipynb`: Jupyter notebook containing the model training and evaluation code.
* `df.pkl`: Pickled dataset used for training the model.
* `pipe.pkl`: Pickled machine learning pipeline used for making predictions.
* `laptop_data.csv`: CSV file containing the raw laptop specifications and prices.
* `requirements.txt`: File listing the required Python packages for the project.
## Installation

To set up the project locally, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/Ananthateja23/Laptop-Price-Predictor.git
   cd Laptop-Price-Predictor
   ```

2. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

To run the application locally:

```bash
streamlit run app.py
```

This command will start a local server and open the application in your default web browser.

## Deployment

You can deploy this Streamlit app on **Render** by following these steps:

1. **Sign up / Log in** to [Render](https://render.com/).

2. **Create a new Web Service**:

   * Click on **New** → **Web Service**.
   * Connect your GitHub account and select the repository: `Laptop-Price-Predictor`.

3. **Configure the service**:

   * **Environment**: Python 3
   * **Build Command**:

     ```bash
     pip install -r requirements.txt
     ```
   * **Start Command**:

     ```bash
     streamlit run app.py --server.port $PORT --server.address 0.0.0.0
     ```

4. **Deploy the service**:

   * Click **Create Web Service** and Render will automatically build and deploy your app.
   * Once deployed, you will get a public URL where anyone can access your Laptop Price Predictor app.

**Tip**: Make sure your `requirements.txt` file includes all necessary dependencies for Streamlit and model prediction.



