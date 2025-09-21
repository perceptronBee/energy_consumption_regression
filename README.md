# Energy Consumption Regression

## 📘 Project Overview

This project focuses on predicting energy consumption in buildings using various regression models implemented in Python. The dataset used is the [Energy Consumption Dataset - Linear Regression](https://www.kaggle.com/datasets/govindaramsriram/energy-consumption-dataset-linear-regression), which includes features related to building characteristics and environmental factors.

## 📊 Dataset Summary

The dataset contains the following columns:

- `Building Type`: Type of the building (e.g., Residential, Commercial)
- `Weekday/Weekend`: Indicates whether the day is a weekday or weekend
- `Temperature`: Ambient temperature in Celsius
- `Humidity`: Ambient humidity percentage
- `Energy Consumption`: Target variable representing energy consumption in kWh

## 🛠️ Project Workflow

1. **Data Loading and Exploration**
   - Loaded the dataset and performed initial exploration to understand its structure and identify any missing values.

2. **Data Preprocessing**
   - Handled missing values appropriately.
   - Encoded categorical variables using Label Encoding and One-Hot Encoding where necessary.
   - Scaled numerical features using StandardScaler to normalize the data.

3. **Modeling**
   - Split the data into training and testing sets.
   - Applied various regression models:
     - Linear Regression
     - Lasso Regression
     - Ridge Regression
     - ElasticNet Regression
   - Evaluated models using metrics such as R², Mean Absolute Error (MAE), and Mean Squared Error (MSE).

4. **Results and Observations**
   - Linear Regression performed best on this dataset.
   - Regularized models like Lasso and ElasticNet showed slightly higher errors due to over-penalization, indicating that simpler models can sometimes outperform regularized ones when overfitting is not a major concern.

## 🚀 How to Run the Code

1. **Clone the repository**
   ```bash
   git clone https://github.com/perceptronBee/energy_consumption_regression.git
   
2. **Navigate to the project folder**
   ```bash
   cd energy_consumption_regression

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt

4. **Open the notebook in Jupyter**
   ```bash
   jupyter notebook energy-consumption.ipynb
