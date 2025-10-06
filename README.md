# 🌱 Crop Yield Prediction

A machine learning project that predicts crop yield based on historical agricultural data, environmental factors, and fertilizer usage. This repository contains the complete pipeline for data preprocessing, model training, evaluation, and a user-friendly web application for making predictions.

## 📖 Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
  - [Running the Jupyter Notebook](#running-the-jupyter-notebook)
  - [Running the Web App](#running-the-web-app)
- [Methodology](#methodology)
  - [Data Preprocessing](#data-preprocessing)
  - [Models](#models)
- [Results](#results)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)

## 🎯 Overview

This project aims to build a predictive model for crop yield, which is crucial for farmers, agricultural planners, and policymakers. By leveraging machine learning, we can forecast production, optimize resource allocation, and enhance food security. The solution includes both a data analysis notebook and an interactive Streamlit web application.

## 📊 Dataset

The primary dataset used is `yield_df.csv`, which contains historical agricultural data. Key features include:
- **Area:** The country or region where the crop was grown.
- **Item:** The type of crop (e.g., Maize, Wheat, Rice).
- **Year:** The year of harvest.
- **hg/ha_yield:** The target variable, representing yield in hectograms per hectare.
- **Average Rainfall:** Annual rainfall in the area.
- **Pesticides:** Pesticides used (in tonnes).
- **Avg Temperature:** Average annual temperature.

A second dataset, `fertilizer.csv`, is used to enrich the data with information on specific fertilizer usage (e.g., Nitrogen, Phosphate, Potash).

## 🔬 Methodology

### Data Preprocessing

- **Handling Missing Values:** Strategies were applied to fill or remove missing data.
- **Encoding Categorical Variables:** Used Label Encoding for categorical features like 'Area' and 'Item'.
- **Feature Engineering:** Created new features and merged the fertilizer dataset to enhance predictive power.
- **Data Splitting:** The data was split into training and testing sets to evaluate model performance.

### Models

Several regression algorithms were implemented and evaluated, including:
- **Linear Regression**
- **Decision Tree Regressor**
- **Random Forest Regressor**
- **Gradient Boosting Regressor**
- **Support Vector Regressor (SVR)**

The **Random Forest Regressor** was identified as the best-performing model based on evaluation metrics and was saved for use in the web application.

## 📈 Results

The performance of the models was evaluated using metrics such as **R-squared (R²)**, **Mean Absolute Error (MAE)**, and **Root Mean Squared Error (RMSE)**. The Random Forest model consistently outperformed others, providing a robust and accurate prediction of crop yield.

*(Note: Specific results, charts, and metrics should be detailed within the Jupyter Notebook.)*

## 🛠️ Technologies Used

- **Python**
- **Pandas & NumPy** (Data Manipulation)
- **Scikit-learn** (Machine Learning Models)
- **Matplotlib & Seaborn** (Data Visualization)
- **Streamlit** (Web Application Framework)
- **Jupyter Notebook** (Interactive Development)
