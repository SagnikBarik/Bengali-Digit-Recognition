# **Bengali Digit Recognition**  

This repository contains the implementation of a Bengali Digit Recognition model using machine learning techniques. The model is trained to recognize Bengali digits from images and has been optimized for deployment in real-world applications.  

## **Dataset**  
The dataset used for this project is from Kaggle and can be found at the following link:  
[**Bengali Digit Dataset**](https://www.kaggle.com/datasets/BengaliAI/numta)  

## **Model Architecture**  
The model is a **Convolutional Neural Network (CNN)** built using TensorFlow/Keras. It consists of:  
- **Conv2D Layers**: Extract spatial features from input images.  
- **MaxPooling Layers**: Reduce dimensionality and improve efficiency.  
- **Flatten Layer**: Converts the feature maps into a 1D vector.  
- **Dropout Layer**: Prevents overfitting by randomly deactivating neurons.  
- **Dense Layer with Softmax Activation**: Outputs probabilities for each digit (0-9).  

The model is trained using **categorical crossentropy** as the loss function and optimized using the **Adam optimizer**.  

## **Data Preprocessing**
Before training, images undergo the following preprocessing steps:  
1. **Grayscale Conversion**: All images are converted to grayscale to reduce complexity.  
2. **Resizing to 28x28 Pixels**: Standardized input size to match CNN requirements.  
3. **Normalization**: Pixel values are scaled to the range [0,1] for improved model performance.  

## **Flutter App Integration**  
The trained model is integrated into a **Flutter-based mobile application** that allows users to draw Bengali digits on a whiteboard and get real-time predictions.  
Check out the Flutter implementation: [**Sonkhya.AI**](https://github.com/SagnikBarik/Sonkhya.AI)  
