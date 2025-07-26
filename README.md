# Handwritten Digit Recognition using CNN (MNIST Dataset)

This project is a Convolutional Neural Network (CNN) implementation in Keras and TensorFlow to classify handwritten digits from the famous [MNIST dataset](http://yann.lecun.com/exdb/mnist/). The model achieves high accuracy in recognizing digits (0–9) and demonstrates core deep learning concepts such as convolution, pooling, dropout, and activation functions.

## 🧠 Project Highlights

- Built using Keras with TensorFlow backend.
- Achieves ~98.7% test accuracy.
- Uses Conv2D, MaxPooling, Dropout, and Dense layers.
- Includes model evaluation, visualization, and prediction.
- Implements EarlyStopping and ModelCheckpoint callbacks for improved training.

## 📁 Dataset

The MNIST dataset is automatically loaded using `keras.datasets.mnist`. It contains:

- **60,000 training images**
- **10,000 testing images**
- Grayscale images of size **28x28 pixels**

## 🛠️ Libraries Used

- `numpy`
- `matplotlib`
- `tensorflow`
- `keras`

## 🧪 Model Architecture

Input Layer (28x28x1 grayscale image)
→ Conv2D → ReLU → MaxPooling
→ Conv2D → ReLU → MaxPooling
→ Flatten
→ Dense (128 units) → ReLU
→ Dropout
→ Dense (10 units - output layer) → Softmax


## 📈 Training

- Optimizer: Adam
- Loss: Categorical Crossentropy
- Epochs: 10 (with EarlyStopping)
- Validation Split: 30%

## 🔍 Evaluation

- Test Accuracy: ~98.7%
- Visualized predictions for sample test images
- Displayed predicted vs actual labels


