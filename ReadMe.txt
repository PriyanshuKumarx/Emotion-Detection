😃 Emotion Detection Using CNN
📌 Overview
This project implements an Emotion Detection System using a Convolutional Neural Network (CNN). It can recognize seven emotions from facial expressions:
😠 Angry | 🤢 Disgust | 😨 Fear | 😃 Happy | 😐 Neutral | 😢 Sad | 😲 Surprise

✨ Features
✔️ Uses Keras with TensorFlow backend for deep learning
✔️ OpenCV for face detection
✔️ Dlib and Haar Cascade for facial landmark detection
✔️ Trains a CNN model to classify emotions from grayscale images
✔️ Real-time emotion detection using a webcam

📂 Dataset Structure
The dataset is structured into labeled directories:

bash
Copy
Edit
dataset/
│-- train/         # 📊 Training images
│-- validation/    # 🔍 Testing images
Each folder contains subdirectories named after emotions, holding respective images.

🏗️ Model Architecture
The CNN model consists of:
🔹 4 convolutional layers (128, 256, 512, 512 filters)
🔹 MaxPooling layers for downsampling
🔹 Dropout layers for regularization
🔹 Dense layers for classification
🔹 Softmax activation for final prediction

🚀 How to Use
🏋️‍♂️ Training the Model
1️⃣ Place your dataset in the appropriate directory structure.
2️⃣ Run the script to preprocess images and train the model.
3️⃣ The trained model is saved as emotiondetector.h5 and emotiondetector.json.

🎭 Running Emotion Detection
1️⃣ Use the trained model to predict emotions from new images.
2️⃣ The script allows testing individual images and real-time webcam detection.
3️⃣ The system displays the detected emotion on the screen.

🎥 Real-time Emotion Detection
To run the webcam-based detection:

bash
Copy
Edit
python emotion_detection.py
This will open a webcam window, detect faces, and classify emotions in real-time.

📜 License
This project is licensed under the MIT License. Unauthorized use, reproduction, or distribution is prohibited.

👤 Author
Priyanshu
