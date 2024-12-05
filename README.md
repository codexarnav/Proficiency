Proficiency Detector 🎯

Overview
This project is a machine learning model that predicts a user's new proficiency level based on their current proficiency, quiz difficulty, and quiz score. The model uses a neural network to estimate how a user's skills might improve after taking a quiz.

Features
Predicts new proficiency levels using a multi-layer neural network
Handles different quiz difficulties (easy, medium, hard)
Provides visualization of model performance
Calculates prediction accuracy using Mean Absolute Error (MAE)


Prerequisites
Python 3.7+
Libraries:
pandas
numpy
scikit-learn
TensorFlow/Keras
matplotlib


Dataset
The model uses a CSV file quiz_proficiency_dataset.csv with the following columns:
current_proficiency: User's initial skill level (0-100)
quiz_difficulty: Difficulty of the quiz ('easy', 'medium', 'hard')
quiz_score: Score achieved in the quiz
new_proficiency: Updated skill level after the quiz


Model Architecture
The neural network consists of:


Input layer: 3 features
Hidden layers:
First layer: 64 neurons (ReLU activation)
Second layer: 32 neurons (ReLU activation)
Third layer: 16 neurons (ReLU activation)



Output layer: 1 neuron (linear activation)
Training
Optimizer: Adam
Loss Function: Mean Squared Error
Epochs: 200
Batch Size: 32
Validation Split: 20%

