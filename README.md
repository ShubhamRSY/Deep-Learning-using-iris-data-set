# Deep Learning using Iris data set

## Description
This repository demonstrates the core deep learning model-building concepts using the Keras library. The Iris flower dataset is used to build a classification model, showcasing key steps such as data preprocessing, model creation, evaluation, and prediction.

---

## Table of Contents
- [What We Did](#what-we-did)
- [Results](#results)
- [Setup](#setup)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Dependencies](#dependencies)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)
- [Notes](#notes)

---

## What We Did
1. **Loaded and Preprocessed the Dataset**:
   - Used columns `Sepal.Length`, `Sepal.Width`, `Petal.Length`, and `Petal.Width` as features.
   - Converted the target column `Species` into numerical categories using a label encoder.
   - Scaled the features and applied one-hot encoding to the target variable.
   - Split the dataset into training and testing sets.

2. **Built and Trained a Neural Network**:
   - Designed a sequential neural network using TensorFlow/Keras.
   - Model architecture:
     - Two dense layers with 128 nodes each and ReLU activation.
     - One softmax output layer for multi-class classification.
   - Training parameters:
     - Epochs: 10
     - Batch size: 16
     - Validation split: 20%
     - Used `categorical_crossentropy` as the loss function and `accuracy` as the metric.

3. **Evaluated the Model**:
   - Achieved a test accuracy of **93.3%** after training.

4. **Made Predictions**:
   - Made single-instance and batch predictions.
   - Decoded predictions back to the original species labels using the label encoder.

---

## Results
### Model Performance:
- **Accuracy**:
  - 93.9% (training)
  - 93.3% (test dataset)
- **Loss**:
  - Final validation loss: 0.34
  - Test dataset loss: 0.24

### Predictions:
- **Example Prediction**:
  - Input: `[6.6, 3.0, 4.4, 1.4]`
  - Output: `'versicolor'`
  - Probabilities: `[0.02, 0.67, 0.31]`

---

## Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Deep-Learning-Example-Iris.git
