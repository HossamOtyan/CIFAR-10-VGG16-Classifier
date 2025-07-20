# CIFAR-10 VGG16 Classifier

A simple image classifier using VGG16 and transfer learning on CIFAR-10 dataset.

## 📋 Description

This project implements an image classification pipeline using TensorFlow and Keras.

It demonstrates transfer learning by using a pre-trained VGG16 model as a fixed feature extractor for classifying CIFAR-10 images.

Only a small subset of the dataset is used (500 training samples and 100 test samples) for faster experimentation and learning purposes.

## 🚀 Features

- Loads CIFAR-10 dataset and selects 500 training and 100 testing images.
- Resizes images from 32x32 to 224x224 pixels to match VGG16 input requirements.
- Uses pre-trained VGG16 model with ImageNet weights as the base model (`include_top=False`).
- Freezes the base model layers (no retraining of VGG16 itself).
- Adds simple dense layers on top for classification into 10 categories.
- Compiles the model with `Adam` optimizer and `categorical_crossentropy` loss.
- Trains for 3 epochs and evaluates accuracy on test data.

## 🛠️ Technologies Used

- Python 3
- TensorFlow / Keras
- Pre-trained VGG16 (ImageNet weights)

## 📦 Notes

- This project is intended as a simple learning example.
- Only a small subset of CIFAR-10 is used (not full dataset training).
- Make sure your environment supports TensorFlow and has enough memory for image resizing and training.

## 📄 License

Feel free to use this code for learning and experimentation.

