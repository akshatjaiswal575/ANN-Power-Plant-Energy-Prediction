# ANN-Power-Plant-Energy-Prediction
An Artificial Neural Network built with PyTorch to predict power plant electrical energy output using environmental and operational features.An Artificial Neural Network built with PyTorch to predict power plant electrical energy output using environmental and operational features.

# Power Plant Energy Output Prediction using ANN

# Project Overview

This project implements an Artificial Neural Network (ANN) using PyTorch to predict electrical energy output from a power plant based on environmental and operational conditions.

The model is trained on a dataset containing ambient temperature, exhaust vacuum, ambient pressure, and relative humidity. The objective is to learn the relationship between these input features and electrical energy output using supervised deep learning.

# Objectives

- Understand and implement an Artificial Neural Network using PyTorch.
- Perform data preprocessing and feature scaling.
- Build a regression model for continuous-value prediction.
- Train the network using backpropagation and the Adam optimizer.
- Evaluate model performance using Mean Squared Error (MSE) and R² score.
- Save and reload the best-performing model weights.

# Dataset

The dataset contains 9,568 records and five columns.

**Input Features:**
- `AT` — Ambient Temperature
- `V` — Exhaust Vacuum
- `AP` — Ambient Pressure
- `RH` — Relative Humidity

**Target Variable:**
- `PE` — Electrical Energy Output

# Model Architecture

The ANN is implemented using PyTorch with the following architecture:

- Input layer: 4 features
- Hidden layer 1: 6 neurons with ReLU activation
- Hidden layer 2: 6 neurons with ReLU activation
- Output layer: 1 neuron for regression

# Technologies Used

- Python
- PyTorch
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

# Workflow

1. Load and inspect the dataset.
2. Check for missing values.
3. Split the dataset into training and testing sets.
4. Scale the input features using StandardScaler.
5. Convert the data into PyTorch tensors.
6. Create TensorDataset and DataLoader objects.
7. Build and train the ANN for 50 epochs.
8. Track training and validation loss.
9. Save and reload the best model weights.
10. Evaluate predictions using MSE and R² score.

# Recorded Results

- Test MSE: approximately 19.57
- R² Score: approximately 0.9316
- Training epochs: 50

These results are from the recorded notebook outputs and should be revalidated after correcting the preprocessing pipeline.

# Project Files

- `ANN_Regression.ipynb` — Data preprocessing, ANN implementation, training, and evaluation.
- `powerplant_data.csv` — Dataset used for training and testing.
- `best_model.pt` — Saved PyTorch model weights.

# Future Improvements

- Correct and validate the feature-scaling pipeline.
- Use a separate validation set and preserve an untouched test set for final evaluation.
- Experiment with different hidden-layer sizes and hyperparameters.
- Build a reusable prediction pipeline for new input samples.
- Compare ANN performance with traditional regression models.

# Learning Outcomes

This project demonstrates practical experience with neural network architecture, supervised regression, model training, loss monitoring, model persistence, and performance evaluation using PyTorch.
