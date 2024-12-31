# Distracted-Driver-Classification
This project focuses on classifying distracted drivers using CNN model.

Overview
This project leverages deep learning to classify driver behavior into various categories based on images, aiming to detect distracted driving. The system processes images of drivers, categorizes them into predefined classes, as shown below, and predicts their activities with high accuracy. The project emphasizes efficient feature extraction and model optimization, achieving robust results even with a relatively low number of epochs and batch size.


The model predicts one of the following ten classes, each describing a specific driver activity:
c0: Safe driving
c1: Texting - right
c2: Talking on the phone - right
c3: Texting - left
c4: Talking on the phone - left
c5: Operating the radio
c6: Drinking
c7: Reaching behind
c8: Hair and makeup
c9: Talking to a passenger


Dataset
The dataset includes images of drivers engaged in ten different activities, as shown above. Each image is resized and preprocessed for training. The dataset is simply shuffled the data to ensure diverse samples for robust model training and testing.


Model Architecture
The model was run on local machine. Initially, a model with 15 epochs was explored, but it was observed that the accuracy and loss stabilized after a few epochs. Therefore, the current model uses a reduced setup of 6 epochs and a batch size of 70, making training efficient without sacrificing performance. (batch size 70 used 27gb ram, increasing batch size would not be recommended)


The model is a Convolutional Neural Network (CNN) built using TensorFlow/Keras, consisting of:
Multiple convolutional layers with ReLU activation and batch normalization.
Max-pooling layers for spatial dimension reduction.
Dropout layers to prevent overfitting.
Dense layers for classification, and softmax layer for output.


Results
With this architecture and data preparation the model achieves high accuracy across all classes while maintaining minimal loss. Visualization techniques includes accuracy/loss plots and confusion matrices, that provide clear insights into the model's performance and areas for improvement.
