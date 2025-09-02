# Assignment-3-AI
# Fashion-MNIST CNN Assignment

**Student Name:** Nada Iyad Mohammed ElKhatib  
**Student ID:** 120220017  
**University:** University of Palestine  
**Major:** Software Engineering  
**Faculty:** Faculty of Software Engineering and Artificial Intelligence  
**Course:** Introduction to Artificial Intelligence  
**Assignment:** 3  

---

## Project Overview

This project implements a **Convolutional Neural Network (CNN)** to classify images from the **Fashion-MNIST dataset**.  
Fashion-MNIST consists of **70,000 grayscale images** of 10 different clothing categories (28x28 pixels each), with 60,000 images for training and 10,000 for testing.  

The goal is to practice deep learning concepts including **loading datasets, visualizing data, building CNN models, training, testing, and saving the trained model**.

---

## Project Phases

### Phase 1: Load Dataset
- Load Fashion-MNIST dataset using TensorFlow/Keras.
- Split into training and testing sets.
- Print shapes of the datasets.

### Phase 2: Display & Visualize Data
- Visualize sample images from the training set.
- Display labels corresponding to the images.

### Phase 3: Build CNN Model
- Normalize pixel values to [0,1].
- Reshape data for CNN input.
- One-hot encode the class labels.
- Define CNN architecture using `Sequential` API:
  - 2 convolutional layers + max pooling + dropout
  - Flatten layer
  - Dense layers with ReLU and softmax output

### Phase 4: Train Model
- Compile CNN with `categorical_crossentropy` loss and `adam` optimizer.
- Save best weights using `ModelCheckpoint`.
- Train for 10 epochs with 10% validation split.
- Optional: Plot training vs. validation accuracy/loss for visualization.

### Phase 5: Test Model
- Load best weights.
- Evaluate model on the test dataset.
- Report **test accuracy**.

### Phase 6: Evaluate & Save Model
- Save the full CNN model to `fashion_mnist_cnn.h5`.

---

## Dataset Information

- Dataset: [Fashion-MNIST](https://github.com/zalandoresearch/fashion-mnist)
- Classes:
  0. T-shirt/top  
  1. Trouser  
  2. Pullover  
  3. Dress  
  4. Coat  
  5. Sandal  
  6. Shirt  
  7. Sneaker  
  8. Bag  
  9. Ankle boot

---

## Dependencies

- Python 3.x  
- TensorFlow (`tensorflow>=2.x`)  
- NumPy  
- Matplotlib  

Install dependencies with:

```bash
pip install tensorflow numpy matplotlib
