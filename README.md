# 🎬 Action Recognition on UCF101 Dataset

## 📌 Overview

This project focuses on human action recognition using the UCF101 dataset, which consists of 101 action categories. The model is built using ResNet-50 as an encoder for feature extraction and LSTM as a decoder to capture temporal dependencies in videos.

The goal is to create an efficient deep learning pipeline that can accurately classify various human activities from video sequences.

**Dataset link :** https://www.crcv.ucf.edu/data/UCF101.php

## 🚀 Features

**✅ 🎥 Video Preprocessing**

Extracts frames from videos and organizes them into a structured format for training.

Converts video data into efficient dataframes for deep learning models.

**✅ 🧠 Deep Learning Model**

ResNet-50 Encoder: Extracts spatial features from video frames.

LSTM Decoder: Captures temporal relationships between frames.

Transfer Learning: Utilizes pretrained ImageNet weights for better performance.

**✅ 📊 Training & Evaluation**

Loss & Accuracy Graphs: Monitors training performance.

Confusion Matrix: Visualizes model performance across action classes.

Classification Report: Includes precision, recall, and F1-score for in-depth evaluation.

**✅ 📈 Optimized Training Strategy**

Uses Adam optimizer for efficient convergence.

Categorical cross-entropy for multi-class classification.

Fine-tuned hyperparameters like batch size, learning rate decay, and dropout layers to prevent overfitting.

## 📖 How It Works?

**1️⃣ Data Processing**

Selects 40 diverse action classes from UCF101.

Converts video data into structured dataframes for training.

Splits dataset into training and validation sets.

**2️⃣ Model Architecture**

ResNet-50 Encoder: Extracts meaningful spatial features.

LSTM Decoder: Captures motion across video frames.

Dense & Dropout Layers: Improves generalization.

**3️⃣ Model Training**

Optimized using Adam optimizer with learning rate decay.

Tracks training/validation loss and accuracy to ensure stability.

**4️⃣ Model Evaluation**

Confusion Matrix for class-wise performance visualization.

Classification Report for detailed precision, recall, and F1-score.

## 📊 Results & Performance

Achieved high accuracy on selected 40 action classes.

Model effectively distinguishes between similar human actions.

Learning curves demonstrate stable training without overfitting.
