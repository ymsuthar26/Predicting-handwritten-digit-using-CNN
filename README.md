# Predicting-handwritten-digit-using-CNN
# Dataset
The MNIST dataset contains:
60,000 training images
10,000 testing images
Each image is 28x28 pixels grayscale, representing digits 0–9.

# Technologies Used
TensorFlow / Keras
Matplotlib
# Project Workflow
1. Data Loading
Loaded MNIST dataset using tf.keras.datasets.mnist.load_data().
2. Data Preprocessing
Normalized pixel values to range [0, 1] by dividing by 255.
Reshaped images to (28, 28, 1) for CNN input.
3. Model Architecture
Conv2D Layer 1: 32 filters, kernel size 3x3, ReLU activation.
MaxPooling2D Layer 1: pool size 2x2.
Conv2D Layer 2: 64 filters, kernel size 3x3, ReLU activation.
MaxPooling2D Layer 2: pool size 2x2.
Flatten Layer
Dense Layer: 128 neurons, ReLU activation.
Output Layer: 10 neurons, softmax activation.
4. Model Compilation & Training
Loss: Sparse Categorical Crossentropy
Optimizer: Adam
Metric: Accuracy
Trained for several epochs on training data.
5. Evaluation
Evaluated accuracy on test dataset.
Visualized some predictions.
# Results
Test Accuracy: ~99% (typical for CNN on MNIST)
Model correctly classifies most handwritten digits.
