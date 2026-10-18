
# Task 3: Multi-Class Image Classification Using CNN

## 1. Project Overview
This project implements a Convolutional Neural Network (CNN) to classify images into ten categories using the CIFAR-10 dataset and TensorFlow/Keras.

## 2. Objectives
- Load and inspect the CIFAR-10 dataset.
- Normalize image pixel values.
- Prepare labels for multi-class classification.
- Build a CNN with convolutional, max-pooling, and fully connected layers.
- Apply data augmentation to help reduce overfitting.
- Plot training and validation accuracy curves.
- Evaluate the model on test data.
- Save the trained model.

## 3. Dataset
Dataset Name: CIFAR-10

The dataset contains 60,000 color images of size 32 × 32 pixels.

- Training images: 50,000
- Testing images: 10,000
- Number of classes: 10

Classes include airplane, automobile, bird, cat, deer, dog, frog, horse, ship, and truck.

The dataset is loaded using TensorFlow/Keras.

## 4. Requirements
- Python
- TensorFlow
- NumPy
- Pandas
- Matplotlib

Install the required libraries:

```bash
pip install tensorflow numpy pandas matplotlib
```

## 5. CNN Architecture
The model contains:

1. Data augmentation
2. Conv2D layers with ReLU activation
3. MaxPooling2D layers
4. Flatten layer
5. Dense layer with 128 neurons
6. Dropout layer
7. Output layer with 10 neurons and softmax activation

## 6. Data Preprocessing
Image pixel values are converted from the range 0–255 to 0–1.

Labels are converted into one-hot encoded vectors for ten-class classification.

Data augmentation uses random horizontal flipping and translation to provide varied training examples and help reduce overfitting.

## 7. Model Training
- Optimizer: Adam
- Loss Function: Categorical Cross-Entropy
- Evaluation Metric: Accuracy
- Epochs: 10
- Batch Size: 64
- Validation Split: 20%

## 8. Evaluation
The model is evaluated using test loss and test accuracy.

Training and validation accuracy curves are plotted to analyze learning performance. Training and validation loss curves are also generated.

Actual results must be recorded after running the Python notebook.

## 9. Output Files
- cifar10_cnn_model.keras: Saved trained CNN model.
- Training and validation accuracy graph.
- Training and validation loss graph.
- Actual-versus-predicted image visualization.

## 10. How to Run
1. Open the notebook in Jupyter Notebook or Google Colab.
2. Install the required libraries.
3. Run all code cells in order.
4. Wait for the CNN training process to finish.
5. Review the accuracy and loss graphs.
6. Check the final test accuracy.
7. Confirm that the model file was saved.

## 11. Conclusion
This project demonstrates a complete image classification pipeline using a CNN. It includes dataset loading, image normalization, data augmentation, CNN architecture design, model training, evaluation, visualization, and model saving.

## 12. References
- CIFAR-10: https://www.cs.toronto.edu/~kriz/cifar.html
- TensorFlow CIFAR-10: https://www.tensorflow.org/api_docs/python/tf/keras/datasets/cifar10
- TensorFlow Conv2D: https://www.tensorflow.org/api_docs/python/tf/keras/layers/Conv2D
