# Bird-Species-classification-using-Sound-
🐦 Bird Species Identification Using Deep Learning
📌 Project Overview

This project presents a Deep Learning-based Bird Species Identification System that classifies bird species from their audio recordings. The model is trained on bird vocalizations from 114 different bird species using Mel-Frequency Cepstral Coefficients (MFCCs) as audio features and a 1D Convolutional Neural Network (CNN) for classification.

The system automatically extracts meaningful audio features from bird sounds and predicts the corresponding bird species with high accuracy. This project demonstrates the application of deep learning in bioacoustics, wildlife monitoring, and environmental conservation.

🚀 Features
Classifies 114 bird species from audio recordings.
Automatic audio preprocessing using Librosa.
MFCC feature extraction for robust sound representation.
Deep Learning model built using TensorFlow/Keras.
1D CNN architecture optimized for audio classification.
Training, validation, and testing pipeline using TensorFlow Dataset API.
Saves trained model and label mappings for future predictions.
Supports prediction on unseen bird audio files.
📂 Dataset

The project uses the Sound of 114 Species of Birds Till 2022 dataset available on Kaggle.

The dataset contains:

Audio recordings (.mp3)
114 different bird species
Organized species-wise into separate folders

Dataset is downloaded using the opendatasets library.

⚙️ Technologies Used
Python
TensorFlow / Keras
Librosa
NumPy
Pandas
OpenCV
Matplotlib
Scikit-learn
tqdm
🧠 Model Architecture

The model consists of:

Input Layer
Conv1D Layer (128 filters)
Batch Normalization
MaxPooling1D
Conv1D Layer (256 filters)
Batch Normalization
MaxPooling1D
Fully Connected Dense Layers
Softmax Output Layer (114 Classes)

Loss Function:

Sparse Categorical Crossentropy

Optimizer:

Adam

Evaluation Metric:

Accuracy
🔍 Workflow
Download bird audio dataset.
Load audio files using Librosa.
Extract MFCC features.
Convert features into TensorFlow tensors.
Encode bird species labels.
Split data into Training, Validation, and Test sets.
Train the 1D CNN model.
Evaluate model performance.
Save trained model and label mapping.
Predict bird species from new audio recordings.
📊 Results

The model is capable of learning discriminative audio features from bird vocalizations and accurately classifying bird species from unseen audio samples. Training and validation accuracy/loss curves are generated to monitor model performance during training.
