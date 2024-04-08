# FlameVision: Wildfire Classification and Detection using Aerial Imagery

FlameVision is a comprehensive aerial image dataset designed specifically for detecting and classifying wildfires. It consists of a total of 8600 high-resolution images, with 5000 images depicting fire and the remaining 3600 images depicting non-fire scenes. The images are provided in PNG format for classification tasks and JPG format for detection tasks. The dataset is organized into two primary folders, one for detection and the other for classification, with further subdivisions into train, validation, and test sets for each folder.

## Overview

In this project, we implemented three different models for wildfire classification using FlameVision dataset: Artificial Neural Network (ANN), Convolutional Neural Network (CNN), and Transfer Learning with VGG16.

### Artificial Neural Network (ANN)

The ANN model was designed for binary classification of 64x64 resized color fire images. The network architecture includes Flatten layer, two Dense layers with ReLU activation, and an output layer with sigmoid activation. 

### Convolutional Neural Network (CNN)

The CNN model was also designed for binary classification of 64x64 resized color images. The architecture includes two Conv2D layers with ReLU activation, MaxPooling layers, Flatten layer, a Dense layer with ReLU activation, and an output layer with sigmoid activation. 

### Transfer Learning with VGG16

We utilized transfer learning with VGG16, a pre-trained model on the ImageNet dataset, for binary classification. The VGG16 base was combined with additional layers, including Flatten and Dense layers. 

## Dataset Preprocessing

We performed data augmentation techniques such as shear, zoom, and horizontal flipping during training to introduce controlled distortions and increase model robustness. The images were resized to 64x64 to reduce training time.

## Conclusion

FlameVision dataset, along with the implemented models, provides a valuable tool for wildfire detection and classification using aerial imagery. The achieved accuracies demonstrate the effectiveness of the proposed approaches in identifying fire incidents.

