🌿 Plant Leaf Disease Detection using CNN

A deep learning project that detects plant leaf diseases using a Convolutional Neural Network (CNN) built with TensorFlow and Keras.
The model is trained on the PlantVillage dataset to classify plant leaves into disease categories.

This project demonstrates a complete deep learning pipeline including:

Dataset loading

Data preprocessing

Data augmentation

CNN model training

Model evaluation

Prediction and visualization

📌 Project Overview

Plant diseases can significantly reduce crop productivity. Early detection helps farmers take preventive actions.

This system uses computer vision and deep learning to automatically classify plant leaf images into disease categories.

The model is trained to classify images into three classes:

Early Blight

Late Blight

Healthy

🧠 Model Architecture

The model is built using TensorFlow / Keras Sequential API.

Architecture

Image Resizing & Normalization

Data Augmentation

Convolution Layers

Max Pooling Layers

Fully Connected Layers

Softmax Output Layer

Example layers used:

Conv2D

MaxPooling2D

Data Augmentation (Flip, Rotation)

Dense layers

📂 Dataset

The model is trained using the PlantVillage Dataset.

Dataset structure:

PlantVillage/
│
├── Early_Blight/
│   ├── image1.jpg
│   ├── image2.jpg
│
├── Late_Blight/
│   ├── image1.jpg
│   ├── image2.jpg
│
├── Healthy/
│   ├── image1.jpg
│   ├── image2.jpg

Dataset is loaded using:

tf.keras.preprocessing.image_dataset_from_directory()
⚙️ Technologies Used

Python

TensorFlow

Keras

NumPy

Matplotlib

Jupyter Notebook

🔄 Data Processing Pipeline

Load dataset using TensorFlow

Split dataset into:

Training set (80%)

Validation set (10%)

Test set (10%)

Apply preprocessing:

Image resizing

Pixel normalization

Apply data augmentation:

Random flip

Random rotation

🚀 Model Training

Training configuration:

Image Size : 256 x 256
Batch Size : 32
Epochs     : 50
Channels   : 3 (RGB)

Loss Function:

SparseCategoricalCrossentropy

Optimizer:

Adam

Evaluation Metric:

Accuracy
📊 Model Evaluation

After training, the model is evaluated using the test dataset.

Metrics monitored:

Training Accuracy

Validation Accuracy

Training Loss

Validation Loss

Graphs are plotted using Matplotlib to visualize training performance.

🔍 Prediction Example

The model predicts the disease class of a leaf image.

Example output:

Actual Label: Early Blight
Predicted Label: Early Blight
Confidence: 98.45%

Prediction function:
