---
title: "Handwriting and CAPTCHA OCR"
excerpt: "both these codes are using a CNN-RNN model with a CTC loss layer to handle sequence prediction. The models achieved over 99% accuracy in recognizing variable-length character sequences from images."
collection: portfolio
---

## Overview

This project implements two different applications: **Handwriting Recognition** and **CAPTCHA OCR**. Both projects share the same model architecture, including a Convolutional Neural Network (CNN) for feature extraction and a Recurrent Neural Network (RNN) with a Connectionist Temporal Classification (CTC) layer for sequence prediction. The CTC layer is critical for handling variable-length sequences and allows the model to make accurate predictions without needing pre-segmented data. Both models achieve more than 99% accuracy.

## Common Architecture

The core model consists of:

- **CNN Layers**: Two convolutional layers followed by max-pooling layers for extracting features from input images.
- **Reshape and Dense Layers**: The output is reshaped and passed through a dense layer to reduce dimensions.
- **RNN Layers**: Two bidirectional LSTM layers are employed to learn temporal dependencies in the input sequence.
- **CTC Layer**: The CTC loss layer is used for training the model to predict sequences of characters efficiently, handling variable-length outputs without explicit alignment.

## Handwriting Recognition

The **Handwriting Recognition** model is trained on the IAM dataset, consisting of images of handwritten words. The images are resized and normalized before feeding them into the model. The CTC layer enables the model to predict characters from sequences without requiring manually segmented inputs. This allows the model to learn and generalize over complex handwritten inputs, achieving more than 99% accuracy.

The model was tested on unseen data, and the accuracy was confirmed with mean edit distance metrics, demonstrating excellent generalization capabilities. The results were visualized with the model correctly predicting sequences for handwritten word images.

## CAPTCHA OCR

The **CAPTCHA OCR** model is trained on a synthetic dataset of CAPTCHA images. These CAPTCHA images are more challenging because of noise, distortion, and variations in character length. Despite these challenges, the architecture based on CNN, RNN, and CTC proved robust, yielding over 99% accuracy on validation data.

This model predicts the sequence of characters in CAPTCHA images without any pre-segmentation and handles noise effectively. The accuracy was verified by comparing the predicted outputs against the ground truth labels. Incorrect predictions were analyzed visually to further improve performance.

## ScreenShots

Screenshots showcasing the results for both projects are included below.
For full code and further details, visit [Captcha GitHub repository](https://github.com/Orgonah/Captcha-OCR-CNN-RNN) and [Handwriting GitHub repository](https://github.com/Orgonah/Handwriting-Recognition)
