# Emotion Detection Using CNN

## Overview
This project implements an emotion detection system using a Convolutional Neural Network (CNN). The system is capable of detecting seven different emotions: **Angry, Disgust, Fear, Happy, Neutral, Sad, and Surprise** from facial expressions.

## Features
- Uses **Keras** with **TensorFlow** backend for deep learning
- Utilizes **OpenCV** for face detection
- Employs **Dlib** and **Haar Cascade** for facial landmark detection
- Trains a CNN model to classify emotions from grayscale facial images
- Real-time emotion detection using a webcam

## Dataset
The dataset used for training and validation is structured into labeled directories:
- `train/` - Contains images for training
- `validation/` - Contains images for testing
Each directory contains subfolders named after emotions, with respective images.

## Model Architecture
The model is a **CNN** with the following layers:
- 4 convolutional layers (128, 256, 512, 512 filters)
- MaxPooling layers after each convolution
- Dropout layers for regularization
- Dense layers for classification
- Softmax activation for final classification

## How to Use
### Training the Model
1. Place your dataset in the appropriate directory structure.
2. Run the script to preprocess images and train the model.
3. The trained model is saved as `emotiondetector.h5` and `emotiondetector.json`.

### Running the Emotion Detector
1. Use the trained model to predict emotions from new images.
2. The script allows testing individual images and real-time webcam detection.
3. The system displays the detected emotion on the screen.

## Real-time Emotion Detection
To run the webcam-based detection:
```bash
python emotion_detection.py
```
This will open a webcam window, detect faces, and classify the emotions in real-time.

## Example Output
The model predicts and displays:
- **Original emotion label** (from the dataset folder structure)
- **Predicted emotion label**
- **Grayscale image visualization**

##License

This project is licensed under the MIT License. Unauthorized use, reproduction, or distribution of this project without proper permission is strictly prohibited and may result in necessary actions.


## Author
Priyanshu

---
Feel free to contribute or provide feedback!

