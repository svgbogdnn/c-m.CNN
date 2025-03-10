# c-m CNN

## Overview

c-m CNN is a comprehensive repository that explores and implements cross-modal convolutional neural network architectures specifically designed for image classification on the CIFAR-10 dataset. By leveraging cross-connections between different color channels in the YUV color space, svgCNN aims to enhance feature extraction and improve overall model performance. The repository provides multiple model variants along with visualization and preprocessing utilities, making it an ideal resource for researchers and practitioners interested in advanced convolutional architectures and cross-modal feature fusion.

## Main Components

- **Model Variants:**  
  The repository includes several implementations of convolutional networks:
  - A 4-layer CNN designed to test basic cross-modal interactions.
  - FitNet-based models that incorporate deeper architectures inspired by the FitNet4 network.
  - A multilayer variant that further explores cross-connections between channels, aiming for richer feature representations.
  
- **Cross-Modal Architecture:**  
  A distinctive feature of c-m CNN is the use of cross-connections between channels. The models split the input into Y, U, and V channels and apply dedicated convolutional layers to each. Later, these channels are merged to facilitate cross-modal information sharing, enabling the network to capture complementary features across different color modalities.

- **Preprocessing Utilities:**  
  The repository offers scripts to convert CIFAR-10 images from RGB to YUV format, ensuring that the network processes data in a format that highlights luminance and chrominance differences. Additionally, utility functions handle data augmentation, normalization, and splitting of the dataset into training and test sets.

- **Visualization Tools:**  
  Alongside the model implementations, c-m CNN includes visualization scripts that generate feature maps at various network stages. Tools for palette generation allow users to assign colors to different layers of feature maps, facilitating qualitative analysis of how cross-modal connections influence learned representations.

- **Training and Logging:**  
  The repository provides scripts for training the networks using real-time data augmentation, with support for saving model weights and logging performance metrics. These tools help track the progress of experiments and enable systematic evaluation of model improvements.

- **Code Organization and Modularity:**  
  The code is organized in a modular fashion, with separate files for different model architectures, preprocessing routines, and visualization functions. This structure makes it easier to modify, extend, or replace individual components, fostering experimentation with novel cross-modal fusion techniques.

## Use Cases and Applications

c-m CNN is designed not only as a proof-of-concept for cross-modal CNN architectures but also as a practical toolkit for:
- Enhancing image classification tasks by leveraging additional color information.
- Studying the effects of cross-channel interactions in convolutional networks.
- Providing a framework for visualization of intermediate features, aiding in model interpretability.
- Serving as a starting point for researchers interested in developing new deep learning models that utilize cross-modal data fusion.

## Getting Started

### Prerequisites

- **Frameworks and Libraries:**  
  - Keras (with TensorFlow backend)  
  - Numpy, Scipy, and PIL for image processing  
- **Dataset:**  
  - CIFAR-10 (automatically loaded and preprocessed via the provided utilities)
- **Environment Setup:**  
  Follow the repository instructions to install necessary dependencies and set up your environment.
