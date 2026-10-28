Airbnb Price Prediction Using LightGBM

About the Project

A machine learning project that predicts Airbnb listing prices using listing details, location, availability, host information, and review-related features. The project uses LightGBM Regression with Scikit-learn preprocessing pipelines for data preparation, model training, and evaluation.

Technologies Used

Python

Pandas and NumPy

Scikit-learn

LightGBM

Matplotlib

Seaborn

Jupyter Notebook

Dataset

Initial records: 102,599

Records with valid prices: 102,352

Input features: 19

Target variable: price

Train-test split: 80:20

The dataset contains listing prices, service fees, room types, neighbourhoods, geographical coordinates, reviews, availability, and host information.

Project Workflow

Data Loading: Loaded and explored the Airbnb dataset using Pandas.

Data Cleaning: Converted numeric columns, handled invalid values, and parsed review dates.

Feature Engineering: Created a days_since_last_review feature.

Preprocessing: Applied median imputation to numerical features and most-frequent imputation to categorical features.

Categorical Encoding: Used One-Hot Encoding and grouped less frequent categories into an Other category.

Model Training: Trained a LightGBM regression model with 600 estimators and a learning rate of 0.05.

Evaluation: Measured performance using Mean Absolute Error (MAE) and R².

Visualization: Generated prediction plots, residual analysis, a correlation heatmap, and feature importance charts.

Model Performance

Metric

Result

Mean Absolute Error (MAE)

2.96

R² Score

0.9968

These are the results from the current experiment. Further validation is needed because the unusually high R² score may indicate target leakage or other evaluation issues.

Key Features

Airbnb price prediction using LightGBM Regression

Automated numerical and categorical preprocessing

Review-date feature engineering

Feature importance analysis

Actual vs. predicted price visualization

Residual error analysis

Numerical correlation heatmap

Installation

Install the required libraries:

pip install pandas numpy scikit-learn lightgbm matplotlib seaborn jupyter

How to Run

Clone or download this repository.

Place the dataset file airbnd.csv in the project directory.

Open the Jupyter Notebook.

Run the cells sequentially to preprocess the data, train the model, evaluate results, and generate visualizations.

Project Structure

airbnb-price-prediction/
├── README.md
├── airbnb_price_prediction.ipynb
├── airbnd.csv
└── requirements.txt

Future Improvements

Investigate potential target leakage and validate performance using cross-validation.

Compare LightGBM with other regression algorithms.

Apply hyperparameter tuning.

Evaluate performance on unseen or more recent listings.

Develop a simple web application for interactive price predictions.

Disclaimer

This project is intended for educational and machine learning practice purposes. Predictions depend on the quality and representativeness of the dataset.

Author: Architha Chepuri
