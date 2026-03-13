Facial Expression Detection using CNN
Overview

This project implements a real-time facial expression detection system using Convolutional Neural Networks (CNN) and OpenCV. The system captures video from a webcam, detects faces using Haar Cascade classifiers, and predicts human emotions using a trained deep learning model.

Facial expression recognition plays an important role in human-computer interaction, healthcare monitoring, and behavioral analysis.

Features

Real-time emotion detection using webcam

Deep learning based facial expression classification

CNN model trained on facial expression dataset

Face detection using Haar Cascade classifier

Visualization of training accuracy and loss

Emotions Detected

The model classifies faces into 7 emotional categories:

Angry

Disgusted

Fearful

Happy

Neutral

Sad

Surprised

Technologies Used

Python

TensorFlow / Keras

OpenCV

NumPy

Matplotlib

Deep Learning (CNN)

Model Architecture

The CNN architecture used in this project consists of:

Convolutional Layers

Max Pooling Layers

Dropout Layers

Fully Connected Dense Layer

Softmax Output Layer (7 classes)

Input image size:

48 × 48 grayscale
Training

The model is trained using a facial expression dataset with approximately:

Training images: 28709
Validation images: 7178

Training parameters:

Epochs: 5
Batch Size: 64
Optimizer: Adam
Loss Function: Categorical Crossentropy
Training Results

The graph below shows the training vs validation accuracy across epochs.

The model achieved approximately:

Validation Accuracy ≈ 56%
Project Structure
Expression-Detection
│
├── model
│   ├── expressionmodel_50.h5
│   └── haarcascade_frontalface_default.xml
│
├── results
│   ├── Epoc_5.png
│   └── plot.png
│
├── ExpressionInit.py
├── TrainCNNModel.py
├── requirements.txt
└── README.md
Installation

Clone the repository:

git clone https://github.com/YOUR_USERNAME/expression-detection.git

Install dependencies:

pip install -r requirements.txt
Run Emotion Detection

Run the following command:

python ExpressionInit.py

This will start the webcam and detect facial emotions in real time.

Applications

Human computer interaction

Mental health monitoring

Smart surveillance systems

Emotion-aware AI assistants

Customer behavior analysis

Future Improvements

Improve model accuracy using deeper CNN architecture

Use transfer learning models (ResNet, MobileNet)

Deploy as a web application

Integrate with real-time video analytics systems

Author

Shreya Raut

License

This project is developed for academic and research purposes.