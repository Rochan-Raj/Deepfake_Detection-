## Deepfake Detection Using Meso4 CNN 

This repository contains an image-based deepfake detection system implemented using the Meso4 Convolutional Neural Network (CNN) architecture.

The work is inspired by the research paper:

https://arxiv.org/pdf/1809.00888

While the original paper focuses on video-based deepfake detection, this project adapts and implements the Meso4 model for still images, making it suitable for image-level deepfake classification.
This project demonstrates to classify whether the given set of images is real or fake. The classification model is based on MesoNet CNN, that includes auto encoders and decoders to produce results using sigmoid function to decide the results in range of 0 to 1. The respective threshold is being set to 0.5, if the resultant value is <0.5 then the image is fake. else its real.

## Project Overview

Deepfake generation techniques have rapidly evolved, making it difficult to distinguish between real and manipulated media. This project aims to:

1.Implement the Meso4 CNN architecture 

2.Detect real vs deepfake facial images

3.Provide a lightweight and efficient model suitable for image-based inference

4.Serve as an educational and experimental extension of the original MesoNet paper

## Model Architecture – Meso4

The Meso4 model is a shallow CNN designed to capture mesoscopic features, which lie between low-level pixel artifacts and high-level semantic features.

Key Characteristics:

  1.Focuses on mid-level visual artifacts introduced during manipulation
  
  2.Lightweight architecture with fewer parameters
  
  3.Efficient training and inference

Architecture Summary:

  A. 4 Convolutional Layers
  
  B. Batch Normalization
  
  C. ReLU Activation
  
  D. Max Pooling
  
  E. Fully Connected Layers
  
  F. Sigmoid Output (Binary Classification: Real / Fake)
  
## Dataset

  Kaggle
  
## Implementation Details

Framework: TensorFlow / Keras
Loss Function: Binary Cross-Entropy
Optimizer: Adam
Evaluation Metrics:

  1.Accuracy
  
  2.Loss

The implementation closely follows the architecture described in the original paper, with adaptations for image-based input instead of video frames.

## Libraries & Dependencies

The following libraries are used in this project:
  Python 3.x
  
  TensorFlow
  
  Keras
  
  NumPy
  
  Pandas
  
  OpenCV
  
  Matplotlib
  
  Scikit-learn
  
## Results

1.The Meso4 model demonstrates effective performance in distinguishing real vs deepfake images

2.Due to its compact architecture, it trains faster compared to deeper CNNs

3.Suitable for experimental and academic purposes

<img width="1920" height="1080" alt="Screenshot 2025-11-18 212616" src="https://github.com/user-attachments/assets/05de586b-cd64-4178-a2a5-ada14f73c56b" />
<img width="1042" height="726" alt="image" src="https://github.com/user-attachments/assets/0d3c7d40-17cc-432f-bc94-75f521b46ce3" />
<img width="1017" height="711" alt="image" src="https://github.com/user-attachments/assets/504cc459-124c-4f3f-8fb8-a90ab8a079e4" />

## Badges


[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)


