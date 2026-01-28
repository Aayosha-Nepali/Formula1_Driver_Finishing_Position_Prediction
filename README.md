# Formula 1 Race Position Prediction Using Machine Learning
## Project Overview
This project explores the application of machine learning techniques to predict Formula 1 driver finishing positions using historical race data. By integrating multiple Formula 1 datasets (drivers, constructors, circuits, races, and results), the project builds a unified dataset and evaluates the performance of different supervised learning models.

Three regression models were implemented and compared:

### Linear Regression

### Random Forest Regressor

### Artificial Neural Network (ANN)

The goal is not only to achieve accurate predictions, but also to analyse how linear vs non‑linear models capture the complex relationships that influence Formula 1 race outcomes.

## Objectives
Merge multi‑table Formula 1 historical datasets into a single analytical dataset

Perform data cleaning, feature engineering, and preprocessing

Implement and evaluate multiple regression models

Compare model performance using standard evaluation metrics

Demonstrate real‑world applicability of machine learning in sports analytics

## Dataset & Features
The dataset was created by combining several Formula 1 data sources, including:

Drivers

Constructors (teams)

Circuits

Races

Race results

## Key Features Used

Grid position

Driver experience

Driver age

Team strength

Circuit latitude and longitude

Season and round number

Experience group (one‑hot encoded)

The target variable for prediction is:

Finishing position

## Machine Learning Models
### 1. Linear Regression

Used as a baseline model

Provides interpretability but assumes linear relationships

Struggled to capture the complexity of race dynamics

### 2. Random Forest Regressor

Captures non‑linear feature interactions

Improved predictive performance compared to Linear Regression

More robust to feature interactions and noise

### 3. Artificial Neural Network (ANN)

Designed to model complex, non‑linear relationships

Implemented using PyTorch

Further improved through feature scaling and hyperparameter tuning

Achieved the best overall performance among the tested models

## Model Evaluation
Models were evaluated using standard regression metrics:

Mean Absolute Error (MAE)

Root Mean Squared Error (RMSE)

R² Score

The tuned ANN achieved the strongest results, demonstrating the importance of non‑linear modelling when predicting Formula 1 race outcomes.

## Inference & Prediction
The trained models can be used to:

Predict race positions for individual drivers

Perform batch predictions for multiple drivers in a given race scenario

Predictions are constrained to valid Formula 1 finishing positions (1–20), ensuring realistic outputs.

## Real‑World Applications
This project demonstrates how machine learning can support:

Motorsport performance analysis

Strategy and decision‑support tools

Trend analysis for teams, analysts, and broadcasters

Predictions are intended as decision‑support insights, not guaranteed outcomes, as real races are influenced by unpredictable factors such as weather, crashes, and mechanical failures.

## Limitations
Limited by the features available in historical datasets

Does not include weather, pit‑stop strategy, tyre compounds, or telemetry data

Predictions cannot account for real‑time race events

## Future Work
Potential improvements include:

Incorporating weather and tyre strategy data

Using lap‑by‑lap telemetry

Applying time‑series or recurrent neural networks

Expanding to real‑time or rolling‑window prediction systems

## Technologies Used
Python

Pandas, NumPy

Scikit‑learn

PyTorch

Matplotlib / Seaborn

## Project Structure
├── data/                # Raw and processed datasets

├── notebooks/           # Model training and evaluation notebooks

├── models/              # Saved trained models

├── figures/             # Plots and visualisations

├── README.md

 ## Author
Aayosha Nepali

Project: Artificial Intelligence
