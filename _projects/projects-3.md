---
title: "Digit Detection Methods"
excerpt: " These projects explore advanced image processing and deep learning techniques for digit classification and numerical computation using convolutional networks and template matching."
collection: portfolio
---

## Overview

Both projects explore the use of deep learning and image processing techniques for extracting and analyzing visual data. While one leverages a convolutional network for digit classification, the other employs template matching for numerical detection and computation from images. Together, these projects demonstrate a range of capabilities in working with image data for both recognition and arithmetic operations.

## Deep Learning for Digit Classification

The goal of this project is to accurately classify handwritten digits from grayscale images using a deep learning model. The dataset used is the well-known MNIST database, a cornerstone in evaluating image classification algorithms.

A Convolutional Neural Network (CNN) was designed to process the 28x28 pixel input images. Through multiple convolution and pooling layers, the model captures critical features of the handwritten digits before passing them through a fully connected network for classification. To prevent overfitting, a dropout layer was introduced.

- **Network Design**: Two convolutional layers, each followed by pooling, extract spatial hierarchies. The feature maps are then flattened and passed through a dense layer with a softmax activation function to produce digit predictions.
- **Optimization**: The model is trained using cross-entropy loss and an Adam optimizer, which tunes the network weights for maximum accuracy.
  
The model achieved a **99.15% accuracy** on the test data, validating its strong performance in digit recognition tasks. Loss on the test set was remarkably low, highlighting the efficiency of the designed architecture. I have implemented this code with both tensorflow and pytorch.

## Image-Based Numerical Computation

This project automates the detection of Farsi numbers in images based on their color and performs basic arithmetic on the extracted values using MATLAB. This is particularly useful in situations where visual data needs to be quickly interpreted and processed.

The image processing pipeline begins with loading and denoising the input images. Farsi Number templates are then used to identify digits based on color—specifically, blue and red digits are detected. Once detected, the system computes the sum of the blue numbers and subtracts this value from the sum of the red numbers.

- **Detection**: The system uses predefined number templates for accurate detection of digits in images, filtering based on color.
- **Computation**: A straightforward subtraction is performed, where the sum of blue numbers is subtracted from the red numbers.
- **Visualization**: The computed result is displayed visually by inserting a green number beneath the original image. All processed images are saved for future analysis.

The final results are visual and stored for documentation. This solution streamlines image-based numerical calculations and provides an easy-to-understand output.

## ScreenShots

Screenshots showcasing the results for both projects:

**Recognition with tensorflow:**
<br/>
<img src='https://YasinDanesh.github.io/YasinDanesh.github.io/images/Python-Digit.png' alt='Digit Image 1' style="margin-bottom:15px; width: 70%">  

**Recognition with MATLAB:**
<br/>
Input example:
<br/>
<img src='https://YasinDanesh.github.io/YasinDanesh.github.io/images/Matlab-Digit-in.png' alt='Digit Image 2' style="margin-bottom:15px; width: 70%">
<br/>

Denoise and detect Farsi numbers:
<br/>
<img src='https://YasinDanesh.github.io/YasinDanesh.github.io/images/Matlab-Digit-out1.png' alt='Digit Image 3' style="margin-bottom:15px; width: 70%">
<br/>

Subtracts the sum of blue numbers from the sum of  
red numbers and put it below the image in Farsi:
<br/>
<img src='https://YasinDanesh.github.io/YasinDanesh.github.io/images/Matlab-Digit-out2.png' alt='Digit Image 4' style="margin-bottom:15px; width: 70%">
<br/>
<br/>

For full code and further details, visit [MATLAB project](https://github.com/YasinDanesh/Image-Number-Detection-and-Computation), [Tensorflow project](https://github.com/YasinDanesh/Digit-Recognition-CNN) and [Pytorch project](https://github.com/YasinDanesh/MNIST-Classification).
