# Image Classification using Convolutional Neural Networks (CNN)

This project implements a **Convolutional Neural Network (CNN)** using TensorFlow and Keras to perform binary image classification. It demonstrates a complete deep learning pipeline, from structural image data augmentation to training and single-image prediction.

## 📌 Project Overview
Computer vision applications require specialized deep learning architectures to extract spatial features from images. This project walks through building a classic CNN pipeline capable of learning pixel patterns, pooling structural features, flattening representations, and classifying target images into binary categories.

---

## 🗺️ Deep Learning Pipeline Structure

The notebook is divided into four main production phases:
1. **Part 1 - Data Preprocessing**:
   * **Preprocessing the Training set**: Leveraging `ImageDataGenerator` for real-time image augmentation (rescaling, shear transformations, zoom modifications, and horizontal flips) to prevent overfitting.
   * **Preprocessing the Test set**: Rescaling test images to match training dimensions without altering internal distribution properties.
2. **Part 2 - Building the CNN**:
   * Initializing the neural network as a Sequential framework.
   * **Step 1 & 2 - Convolution & Pooling**: Applying feature detectors (filters) followed by Max Pooling to compress spatial size.
   * Adding a second convolutional and pooling layer to extract deeper, high-level structural patterns.
   * **Step 3 - Flattening**: Transforming the 2D feature maps into a 1D vector.
   * **Step 4 & 5 - Full Connection & Output Layer**: Routing features through a Dense hidden layer (`ReLU`) and finalizing with a single output node (`Sigmoid`) for binary classification.
3. **Part 3 - Training the CNN**:
   * Compiling the network using the `adam` optimizer and `binary_crossentropy` loss functions.
   * Fitting the CNN to the augmented image directory over optimized batch training cycles.
4. **Part 4 - Making a Single Prediction**:
   * Loading a raw test image, preprocessing its dimensions to match the \(64 \times 64\) target size, and extracting the binary class prediction.

---

## 🛠️ Prerequisites & Tech Stack

Ensure you have the deep learning ecosystem installed:

```bash
pip install numpy pandas matplotlib tensorflow scikit-learn
```

| Framework / Library | Primary Responsibility |
| :--- | :--- |
| **TensorFlow / Keras** | Core deep learning framework, CNN layer compilation, & ImageDataGenerator |
| **NumPy** | Vectorized matrix operations for target image array parsing |
| **Matplotlib** | Training evaluation curves and image loading visualizations |

---

## 🚀 How to Run the Project

1. Clone this repository:
   ```bash
   git clone https://github.com
   ```
2. Set up your dataset directory structure matching the folder footprints:
   ```text
   dataset/
   ├── training_set/
   └── test_set/
   ```
3. Open `convolutional_neural_network.ipynb` inside **Google Colab** or **Jupyter Notebook**.
4. Run all cells sequentially (`Runtime > Run all` in Colab).

---

## 📄 License
This project is licensed under the MIT License - see the LICENSE file for details.
# Convolutional-Neural-Network-CNN-image-classification-project
