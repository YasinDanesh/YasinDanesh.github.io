---
title: "Image Denoising Techniques"
excerpt: " Innovative methods for image denoising using MATLAB and deep learning techniques. These projects showcase expertise in removing noise and enhancing image quality through advanced filtering and autoencoder models."
collection: portfolio
---

## Overview

This collection features specific image denoising techniques, including a MATLAB algorithm for salt and pepper noise removal and a convolutional autoencoder implemented with Keras to enhance image quality in the MNIST dataset.

## Salt and Pepper Denoising using MATLAB

Developed an advanced denoising algorithm for images affected by salt and pepper (S&P) noise, surpassing the performance of traditional Gaussian and median filters. This project also involved implementing edge detection and thresholding techniques to accurately identify numbers within the images.

**Key Features**

- **Enhanced Denoising**: Utilized innovative methods to effectively remove salt and pepper noise from images.
- **Edge Detection**: Applied edge detection algorithms to enhance the clarity of object boundaries within the images.
- **Thresholding**: Implemented thresholding techniques for precise number detection.

## Image Denoising Using Autoencoder

This project focuses on using a convolutional autoencoder to denoise images, particularly leveraging the MNIST dataset. The deep convolutional autoencoder is designed to transform noisy digit images into clean versions, showcasing a practical application of deep learning in image processing.

**Model Architecture**

Convolutional Autoencoder: Built using Keras Functional API, the model consists of convolutional layers to effectively capture and reconstruct image features.

**Training Process**

1. **Initial Training:** The autoencoder is first trained using clean images for both input and output, allowing it to learn the baseline image features.
2. **Denoising Training:** In the second phase, the model is retrained using noisy images as input and clean images as output, enabling it to learn the denoising process.

## ScreenShots

Screenshots showcasing the results for both projects:

**Denoising with Autoencoder:**
<br/>
<img src='https://YasinDanesh.github.io/images/Denoise_AE.png' alt='Denoise 1' style="margin-bottom:15px; width: 100%">  

**Denoising S&P with filters:**
<br/>
<img src='https://YasinDanesh.github.io/images/Denoise_Matlab.png' alt='Denoise 2' style="margin-bottom:15px; width: 100%">
<br/>
<br/>

For full code and further details, visit [S&P filter project](https://github.com/YasinDanesh/Image-Salt-Pepper-Denoising) and [Autoencoder project](https://github.com/YasinDanesh/Digit-Recognition-CNN).
