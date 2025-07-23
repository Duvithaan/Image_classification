# 🖼Image Classification using CNN

This project demonstrates how to build a **Convolutional Neural Network (CNN)** for classifying images from the **CIFAR-10 dataset**. The dataset contains 60,000 32x32 color images across 10 categories such as airplane, automobile, bird, cat, deer, dog, frog, horse, ship, and truck.

## Dataset

- **CIFAR-10**: Preloaded from `tensorflow.keras.datasets`
- 10 Classes: `airplane`, `automobile`, `bird`, `cat`, `deer`, `dog`, `frog`, `horse`, `ship`, `truck`

## Tech Stack

- **Python 3**
- **TensorFlow / Keras**
- **NumPy**
- **Matplotlib**

##  Model Architecture

- `Conv2D` Layer (32 filters, 3x3 kernel, ReLU activation)
- `MaxPooling2D` Layer (2x2 pool size)
- `Conv2D` Layer (64 filters, 3x3 kernel, ReLU activation)
- `MaxPooling2D` Layer (2x2 pool size)
- `Conv2D` Layer (64 filters, 3x3 kernel, ReLU activation)
- `Flatten` Layer
- `Dense` Layer (64 units, ReLU activation)
- `Dense` Output Layer (10 units, Softmax activation)

## Training Details

- Dataset normalized (divided by 255.0)
- Trained on 20,000 samples for efficiency
- Epochs: 10
- Loss Function: `sparse_categorical_crossentropy`
- Optimizer: `adam`
- Metrics: `accuracy`

## Output

- Accuracy and loss evaluated on testing data
- Visualization of a few input images using `matplotlib`

##  How to Run

1. Clone this repository
2. Install dependencies:
   ```bash
   pip install tensorflow matplotlib numpy
