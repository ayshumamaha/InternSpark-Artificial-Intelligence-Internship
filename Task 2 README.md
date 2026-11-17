# Deep Learning – Image Classification Using Python

## 1. Project Overview

The Deep Learning Image Classification Project is a Python application that uses a neural network to recognize and classify handwritten digits. It uses the Digits dataset available through Scikit-learn, which contains images of handwritten digits represented as 8×8 pixel arrays.

The application uses PyTorch to build and train a Multi-Layer Perceptron (MLP) neural network. The dataset is preprocessed and divided into training and testing sets. The model learns patterns from the training images and predicts digit categories for previously unseen test images.

The project demonstrates deep learning concepts, neural network architecture, model training, evaluation, and prediction using PyTorch.

## 2. Objectives

- Develop a basic deep learning image classification model.
- Understand neural network architecture and training.
- Use PyTorch for model development.
- Preprocess image data and prepare it for training.
- Evaluate model performance using test data.
- Visualize training loss and accuracy.
- Save the trained model for future inference.

## 3. Tools and Technologies Used

- **Programming Language:** Python
- **Deep Learning Framework:** PyTorch
- **Libraries:** NumPy, Matplotlib, Scikit-learn
- **Dataset:** Scikit-learn Digits Dataset
- **Model:** Multi-Layer Perceptron (MLP)
- **Concepts:** Neural networks, image classification, training, testing, inference

## 4. Features Implemented

- Loads the handwritten digits dataset.
- Preprocesses and normalizes image data.
- Divides the dataset into training and testing sets.
- Converts the dataset into PyTorch tensors.
- Builds a neural network using fully connected layers.
- Trains the model using an optimizer and loss function.
- Evaluates the model on test data.
- Displays training loss and accuracy curves.
- Generates a confusion matrix and classification report.
- Saves the trained model as `digit_classifier.pth`.
- Performs inference on a sample image.

## 5. How to Run the Program

1. Install Python on your system.
2. Install the required libraries:

```bash
pip install torch numpy matplotlib scikit-learn
```

3. Save the program as `deep_learning.py`.
4. Open a terminal or command prompt.
5. Navigate to the project folder.
6. Execute the following command:

```bash
python deep_learning.py
```

7. Wait for the neural network to complete its training process.
8. View the evaluation results and training visualizations.
9. The trained model is saved as `digit_classifier.pth`.

## 6. Expected Output

The program displays the training progress, including loss and accuracy for each epoch. After training, it evaluates the model using the test dataset and displays test accuracy, classification metrics, and a confusion matrix.

The application also demonstrates prediction on a sample handwritten digit and saves the trained model in a `.pth` file for later use.

## 7. Learning Outcomes

- Understanding fundamental deep learning concepts.
- Learning how neural networks are structured.
- Working with PyTorch tensors and DataLoaders.
- Training and evaluating a neural network.
- Understanding loss functions and optimizers.
- Visualizing training performance.
- Saving and using a trained model for inference.

## Author

M. Ayshwarya
