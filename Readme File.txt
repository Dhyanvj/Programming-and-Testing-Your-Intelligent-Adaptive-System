Project: Indoor Environment Prediction and Adjustment System

Welcome to the Indoor Environment Prediction and Adjustment System! This project aims to predict indoor environmental conditions and adjust them based on predicted satisfaction levels. The system uses data-driven modeling and machine learning to automate environmental control for indoor spaces. Below is an overview of the project's structure, setup, and key functions.

Requirements
To run this project, you need the following dependencies installed:

Python 3.7 or later
NumPy
Pandas
Matplotlib
Scikit-learn
TensorFlow (with Keras)

Install these packages using pip:
pip install numpy pandas matplotlib scikit-learn tensorflow

Project Structure
- indoor_env.py: The main script containing all the code for data loading, model building, training, evaluation, and environment adjustment.
- train.csv: Training data for the LSTM model.
- test.csv: Test data for making predictions and adjusting indoor conditions.
- predicted_test.csv and predicted_train.csv: Output files storing predicted and adjusted values for test and train datasets, respectively.

Model Training
The LSTM model is trained to predict indoor environmental satisfaction based on various features, including temperature, humidity, CO2 levels, etc. The model is built and trained using the following steps:

- Data Loading: Loads and preprocesses training data, handling missing values and converting satisfaction to a numeric format.
- Feature Scaling: Scales features using MinMaxScaler.
- Model Building: Builds an LSTM model with an Adam optimizer and Huber loss.
- Model Training: Trains the model with training and validation data, tracking the mean squared error (MSE) over 10 epochs.

Model Evaluation
After training, the model is evaluated on a test dataset. The following metrics are calculated:

- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)
- R-squared (R2)
These metrics help gauge the model's accuracy and predictive performance. Additionally, a plot is generated comparing actual and predicted satisfaction levels.

Indoor Environment Adjustment
Based on the model's predictions, the system can adjust indoor environmental conditions. The following functionalities are included:

- Mechanical Ventilation: Simulates mechanical ventilation for indoor temperature and humidity adjustments.
- Storage Heater Availability: Checks if the storage heater can be used based on certain conditions (e.g., time elapsed since last use).
- Environment Adjustment: Adjusts indoor environment based on predicted satisfaction, modifying temperature, humidity, etc.

License
This project is licensed under the MIT License. Feel free to use and modify the code as needed, but please give credit to the original authors.