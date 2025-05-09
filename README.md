# Sign Language Detection Using Deep Learning

This project focuses on detecting static American Sign Language (ASL) alphabet hand gestures using deep learning techniques. The system uses a Convolutional Neural Network (CNN) built on top of ResNet50 with preprocessing, data augmentation, and real-time detection support.

## Project Overview

- **Goal:** Classify 24 ASL hand signs (excluding 'J' and 'Z') from static images.
- **Approach:** Deep CNN & Transfer Learning using ResNet50.
- **Future Scope:** Real-time prediction from webcam input using MediaPipe Hands.

## Dataset

- **Source:** [American Sign Language Dataset](https://www.kaggle.com/datamunge/sign-language-mnist)
- **Preprocessing:**
  - Gaussian Blur
  - Adaptive + Otsu Thresholding
  - Resized to 32×32
  - Normalized to [0, 1]
  - Data Augmentation (rotation, zoom, flip)

## Model Architecture

- **Base Model:** ResNet50 (Transfer Learning)
- **Additional Layers:**
  - Dense layers with ReLU & L2 Regularization
  - Batch Normalization
  - Dropout for regularization

## Training Configuration

- **Optimizer:** Adam
- **Loss Function:** Categorical Crossentropy
- **Scheduler:** Exponential Learning Rate Decay
- **Metrics:** Accuracy
- **Epochs:** 30
- **Validation Accuracy:** ~99%

## Evaluation

- Training/Validation accuracy and loss curves
- Confusion Matrix analysis for class-wise performance
- Generalization observed with minimal overfitting

## Future Work

- Integrate MediaPipe Hands for real-time webcam input
- Sequence prediction to form words
- Deploy as a web or mobile app

## Contributors

- Subhoshri Pal  
- Rounak Kumar Singh  
- Shubham  

**Supervisor:** Prof. Arindam Biswas, IIEST Shibpur

---

