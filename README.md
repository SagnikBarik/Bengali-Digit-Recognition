# **Bengali Digit Recognition**  

This repository contains the implementation of a Bengali Digit Recognition model using machine learning techniques. The model is trained to recognize Bengali digits from images and has been optimized for deployment in real-world applications.  

## **Dataset**  
The dataset used for this project is from Kaggle and can be found at the following link:  
[**Bengali Digit Dataset**](https://www.kaggle.com/datasets/BengaliAI/numta)  

## **Model Architecture**
The model is a **Convolutional Neural Network (CNN)** built using TensorFlow/Keras. It consists of:  
- **Conv2D Layers**: Extract spatial features.
- **MaxPooling Layers**: Reduce dimensionality.
- **Flatten Layer**: Converts feature maps into 1D vector.
- **Dropout Layer**: Prevents overfitting.
- **Dense Layer with Softmax Activation**: Outputs probabilities for each digit.

Trained with **categorical crossentropy** loss and **Adam optimizer**.

## **Data Preprocessing**
Preprocessing steps:
1. **Grayscale Conversion**
2. **Resizing to 28x28 Pixels**
3. **Normalization**: Pixel values scaled to [0,1].

## **Flutter App Integration**  
The trained model is integrated into a **Flutter-based mobile application** that allows users to draw Bengali digits on a whiteboard and get real-time predictions.  
Check out the Flutter implementation: [**Sonkhya.AI**](https://github.com/SagnikBarik/sonkhya_ai)  
