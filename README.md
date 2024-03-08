# Power-System-Load-Type-Prediction
## Objective:

This project aims to develop a machine learning model capable of automatically predicting the "Load_Type" (Light Load, Medium Load, Maximum Load) of a power system based on historical data.

## Data Description:

The provided dataset includes features essential for understanding and predicting load types:

Date (Continuous-time): Date of data collection (usually first of the month)
Usage_kWh (Continuous kWh): Industry energy consumption
Lagging Current (Continuous kVarh): Reactive power
Leading Current (Continuous kVarh): Reactive power
CO2 (Continuous ppm): Carbon dioxide emissions
NSM (Continuous S): Number of seconds from midnight
Load Type (Categorical): Light Load, Medium Load, Maximum Load
Methodology:

## Data Preprocessing:

Import necessary libraries (pandas, scikit-learn)
Load the dataset
Handle missing values (e.g., imputation, dropping rows)
Create date-time features (year, month, day, hour) from the 'Date' column (if applicable)
Exploratory Data Analysis (EDA):

Visualize data distributions (histograms, boxplots)
Identify potential correlations between features and load type
Feature Engineering:

Create new features based on domain knowledge or EDA insights (e.g., ratios, time-based aggregations)
## Model Selection and Training:

Split data into training and testing sets, using the last month's data for testing (validation strategy)
Train a Random Forest Classifier model on the training data
Consider alternative models (e.g., Support Vector Machines, Neural Networks) based on complexity and performance
Model Evaluation:

## Evaluate the model's performance on the unseen test data using classification metrics:
Accuracy: Proportion of correct predictions
Precision: Ratio of true positives to predicted positives (avoiding false positives)
Recall: Ratio of true positives to actual positives (avoiding false negatives)
F1-score: Harmonic mean of precision and recall
Code Structure:

## The code is likely organized into functions or scripts for:

Data loading and preprocessing
Feature engineering
Model training and evaluation
## Usage:

Clone or download the repository.
Install required dependencies using pip install <requirements.txt>.
Run the main script (e.g., python main.py) to train and evaluate the model.
Further Exploration:

Experiment with different feature engineering techniques and model architectures.
Implement hyperparameter tuning to optimize model performance.
Integrate the model into a real-time prediction system.
## Conclusion
This project successfully developed a machine learning model for predicting the "Load_Type" (Light Load, Medium Load, Maximum Load) of a power system based on historical data. By employing a Random Forest Classifier and a validation strategy using the last month's data for testing, the model learned to identify patterns in the various features (Usage_kWh, Lagging Current, Leading Current, etc.) and associate them with the corresponding load types.
