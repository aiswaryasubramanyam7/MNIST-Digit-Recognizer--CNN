🧠 MNIST Handwritten Digit Recognizer
📌 Project Overview
This project implements a Convolutional Neural Network (CNN) built with TensorFlow and Keras to classify images of handwritten digits (0-9) using the classic MNIST dataset. It serves as a foundational computer vision model, demonstrating the end-to-end pipeline of data preprocessing, model architecture design, training, and evaluation.

🚀 Features
Automated Data Pipeline: Downloads, reshapes, and normalizes the MNIST dataset (60,000 training images / 10,000 test images).
Custom CNN Architecture: Specifically designed for fast and accurate processing of 28x28 grayscale images.
High Accuracy: Achieves [Enter your final accuracy, e.g., 98.5%] accuracy on unseen test data in just a few epochs.
Live Prediction Test: Includes a script to visually verify the AI's prediction against a random test image.

🏗️ Model Architecture
The neural network uses a sequential architecture divided into two main phases:
Feature Extraction (Convolutional Base):
Conv2D (32 filters, 3x3 kernel) + ReLU activation
MaxPooling2D (2x2)
Conv2D (64 filters, 3x3 kernel) + ReLU activation
MaxPooling2D (2x2)

Classification (Dense Head):
Flatten layer to convert 2D maps to a 1D vector
Dense layer (64 neurons) + ReLU activation
Dense output layer (10 neurons) + Softmax activation for digit probability distribution.

💻 How to Run (Jupyter/Colab)
Clone this repository:
Bash
git clone https://github.com/[aiswaryasubramanyam7]/[MNIST-Digit-Recognizer--CNN].git
Open the .ipynb file in Google Colab or your local Jupyter environment.

Run the cells sequentially to download the data, train the model, and evaluate the predictions.

🔮 Next Steps & Future Scope
Currently, this model runs entirely within a Python notebook environment. The next phase of this project involves converting the model to TensorFlow.js and deploying it as a full-stack web application:

Backend: Node.js server to host the AI model.

Frontend: React application with a drawing canvas where users can draw numbers and receive real-time AI predictions.
