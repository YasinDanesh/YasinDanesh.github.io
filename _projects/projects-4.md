---
title: "Image Denoising Techniques"
excerpt: " Innovative methods for image denoising using MATLAB and deep learning techniques. These projects showcase expertise in removing noise and enhancing image quality through advanced filtering and autoencoder models."
collection: portfolio
---

## Overview

This collection features specific image denoising techniques, including a MATLAB algorithm for salt and pepper noise removal and a convolutional autoencoder implemented with Keras to enhance image quality in the MNIST dataset.

## Salt and Pepper Denoising using MATLAB

Developed an advanced denoising algorithm for images affected by salt and pepper noise, surpassing the performance of traditional Gaussian and median filters. This project also involved implementing edge detection and thresholding techniques to accurately identify numbers within the images.

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

**Recognition with tensorflow:**
<br/>
<img src='https://orgonah.github.io/YasinDanesh.github.io/images/Python-Digit.png' alt='Digit Image 1' style="margin-bottom:15px; width: 70%">
<br/>

**Recognition with MATLAB:**
<br/>
Input example:
<br/>
<img src='https://orgonah.github.io/YasinDanesh.github.io/images/Matlab-Digit-in.png' alt='Digit Image 2' style="margin-bottom:15px; width: 70%">
<br/>
<br/>
Denoise and detect Farsi numbers:
<br/>
<img src='https://orgonah.github.io/YasinDanesh.github.io/images/Matlab-Digit-out1.png' alt='Digit Image 3' style="margin-bottom:15px; width: 70%">
<br/>
<br/>
Subtracts the sum of blue numbers from the sum of
red numbers and put it below the image in Farsi:
<br/>
<img src='https://orgonah.github.io/YasinDanesh.github.io/images/Matlab-Digit-out2.png' alt='Digit Image 4' style="margin-bottom:15px; width: 70%">
<br/>
<br/>
<br/>
For full code and further details, visit [MATLAB project](https://github.com/Orgonah/Image-Number-Detection-and-Computation), [Tensorflow project](https://github.com/Orgonah/Digit-Recognition-CNN) and [Pytorch project](https://github.com/Orgonah/MNIST-Classification)
