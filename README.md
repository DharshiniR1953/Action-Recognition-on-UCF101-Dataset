# Action-Recognition-on-UCF101-Dataset
**1. Data Processing**

Dataset link : https://www.crcv.ucf.edu/data/UCF101.php

Began by selecting a subset of 40 classes from the UCF101 dataset, focusing on a diverse range of actions to ensure robust model training and evaluation.

The video data is preprocessed and converted into dataframes that can be efficiently utilized by our deep learning model.

This conversion involves extracting frames from videos and organizing them in a structured format suitable for training.

Two samples from the dataset, along with their corresponding captions, are plotted to provide a visual reference of the data.

The processed data is split into training and validation sets to facilitate model training and evaluation.

**2. Model Building**


**Encoder - ResNet-50**

The ResNet-50 model is employed as the CNN encoder for feature extraction.

Pretrained weights on ImageNet are used to leverage transfer learning and enhance the model's performance on action recognition.

**Decoder - LSTM**

A 2-layer LSTM model is added as the decoder to capture temporal dependencies in the video sequences.

Additional layers, such as Dense and Dropout, are incorporated to refine the model's predictions and prevent overfitting.

**3. Model Compilation**


The model is compiled using an Adam optimizer with a carefully chosen learning rate to ensure stable and efficient training.

Categorical cross-entropy is selected to measure the discrepancy between the predicted and actual action classes.

Other hyperparameters, such as batch size and learning rate decay, are configured to optimize the model's performance.

**4. Model Training**


The model is trained for a specified number of epochs, with the training process carefully monitored to prevent overfitting and underfitting.

The training and validation loss for each epoch is printed to track the model's learning progress.

The loss and accuracy history graphs for both the training and validation sets are plotted to visualize the model's performance over time.

**5. Model Evaluation**


The trained model is evaluated using a test set, with random samples selected to demonstrate the model's action recognition capabilities.

Confusion Matrix: A confusion matrix is generated to visualize the performance of the model across different action classes.

Classification Report: A detailed classification report, including precision, recall, and F1-score, is printed to provide a comprehensive evaluation of the model's performance.
