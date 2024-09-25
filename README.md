# PixRevive-CNN-Autoencoder-for-Enhanced-Image-Clarity
PixRevive: CNN Autoencoder for Enhanced Image Clarity is a deep learning project that leverages convolutional neural networks (CNNs) to restore blurred images. By training an autoencoder model, PixRevive learns to reconstruct images, improving clarity and revealing complex features for better visual representation.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Acknowledgments](#acknowledgments)

## Project Overview
PixRevive focuses on solving the problem of image blurring by training a CNN autoencoder. The model takes blurred images as input and outputs deblurred versions, enhancing the visual clarity of the images.

## Dataset
The project uses the CIFAR-10 dataset, which consists of 60,000 32x32 color images in 10 different classes. For this project, the images are preprocessed to create blurred versions, which are used to train the autoencoder.

- **Training Data**: Blurred images and their corresponding original (clean) images.
- **Testing Data**: Similar preprocessing on test images to evaluate the model's performance.

## Model Architecture
The CNN autoencoder consists of:
- **Encoder**: A series of convolutional layers to extract image features and reduce spatial dimensions.
- **Latent Space**: A compressed representation of the image features.
- **Decoder**: Convolutional and upsampling layers to reconstruct the image from the latent space.

The model is trained using the Mean Squared Error (MSE) loss function and optimized with the Adam optimizer.
