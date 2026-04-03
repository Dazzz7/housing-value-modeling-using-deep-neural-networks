# Housing Price Intelligence using Deep Learning & Regression
##📌 Overview
End-to-end machine learning project for housing price prediction
Combines:
Exploratory Data Analysis (EDA)
Feature Engineering
Data Validation (TFDV)
Machine Learning & Deep Learning models
Goal: Build a robust and scalable price prediction system

## 📊 Exploratory Data Analysis (EDA)
Dataset understanding:
Shape, structure, data types
Descriptive statistics
Missing value analysis:
Identified missing values in total_bedrooms
Visualization techniques:
Scatter plots (income vs house value)
3D plots (income, rooms, price)
Violin plots (categorical impact)
Heatmaps (correlation analysis)
Pair plots (feature relationships)
Key insights:
Strong correlation between median_income & house price
Geographic trends influence pricing (latitude/longitude)
Most houses fall within mid-range pricing

## 🧹 Data Preprocessing
Missing value handling:
total_bedrooms → filled using mean
Outlier removal:
IQR-based filtering
Feature encoding:
ocean_proximity → Label Encoding
Feature scaling:
StandardScaler applied on train/test data
## ✅ Data Validation (TFDV)
Generated dataset statistics
Schema inference
Anomaly detection
Ensures:
Data consistency
Feature integrity
Production-level reliability

## 🤖 Models Implemented
1. Linear Regression (Baseline)
Implemented using neural network structure
Captures linear relationships
Limitation:
Cannot model complex patterns
2. Multi-Layer Perceptron (MLP)
Architecture:
Input layer → Hidden layers → Output layer
Activation:
ReLU
Benefits:
Captures non-linear relationships
Improved accuracy over LR
3. Deep Neural Network (DNN)
Deep architecture with multiple dense layers
High learning capacity
Captures complex feature interactions
Best overall performance

## ⚙️ Hyperparameter Tuning
Tool: Keras Tuner (Random Search)
Tuned parameters:
Number of layers
Number of neurons per layer
Optimizers: Adam, SGD, RMSprop
Learning rates: 0.01, 0.001, 0.0001
Objective:
Minimize validation Mean Squared Error (MSE)

## 📈 Model Evaluation Metrics
Mean Absolute Error (MAE)
Mean Squared Error (MSE)
Root Mean Squared Error (RMSE)
Explained Variance Score

## 📊 Results Summary
### Linear Regression:
High error, limited performance
### MLP:
Significant improvement
Better generalization
### DNN:
Lowest error
Highest variance score (~0.79)
Best predictive performance

## 📉 Model Diagnostics
Residual analysis
Predicted vs Actual plots
Loss curves visualization
Insights:
DNN captures non-linear trends effectively
Minimal bias in predictions

##🔮 Predictions
Predicts housing prices for unseen data
Supports:
Single-instance predictions
Batch predictions
Real-world applicability in:
Real estate analytics
Investment decision systems

##🚀 Key Highlights
End-to-end ML pipeline
Strong EDA with visual insights
Outlier handling using IQR
Data validation using TFDV
Hyperparameter tuning for optimization
Deep learning applied to tabular data
Model comparison (LR vs MLP vs DNN)
Production-level ML workflow

## 🛠️ Tech Stack: 
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, TensorFlow / Keras, Keras Tuner, TensorFlow Data Validation (TFDV)

Dataset-
california_housing_data*.csv is California housing data from the 1990 US Census; more information is available at:
https://docs.google.com/document/d/e/2PACX-1vRhYtsvc5eOR2FWNCwaBiKL6suIOrxJig8LcSBbmCbyYsayia_DvPOOBlXZ4CAlQ5nlDD8kTaIDRwrN/pub

## Demo:
https://colab.research.google.com/drive/1DatU451jlhfz7TY9xdadhbBxLn0AJfKu#scrollTo=6yD4cC8bZsMc
