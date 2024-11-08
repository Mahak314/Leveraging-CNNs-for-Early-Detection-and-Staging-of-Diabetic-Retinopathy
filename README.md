Diabetic Retinopathy Detection Using CNN

This project implements a Convolutional Neural Network (CNN) model to classify diabetic retinopathy (DR) from retinal images. The project is aimed at automating diabetic retinopathy detection, providing an efficient tool to aid in early diagnosis and treatment.

Table of Contents

Overview

Dataset

Model Architecture

Data Preprocessing

Training and Evaluation

Results

Usage

Dependencies

License

Overview

Diabetic retinopathy is a complication of diabetes that affects the eyes. Early detection and treatment can prevent vision loss. This project classifies retinal images into categories of diabetic retinopathy or no DR.

Dataset

The dataset used is from a drive-mounted directory containing images labeled with severity levels. It includes image files organized into different categories based on the level of diabetic retinopathy.

Model Architecture

The CNN architecture consists of:

-Conv2D Layers: For feature extraction using convolutional filters.

-MaxPooling Layers: For down-sampling, reducing dimensionality.

-Batch Normalization: To stabilize and speed up training.

-Fully Connected Layers: For classification based on extracted features.

Data Preprocessing

-Data Splitting: The dataset is divided into training, validation, and test sets using stratified sampling.

-Image Augmentation: The ImageDataGenerator is used to rescale images and provide real-time data augmentation during training.

-Directory Setup: The images are copied to train/validation/test directories for easy batching.

Training and Evaluation

The model is trained on the processed dataset and evaluated using accuracy, loss, and F1 score metrics.

Evaluation Metrics

Accuracy

Confusion Matrix: To visualize model performance across classes.

F1 Score: To measure model performance, balancing precision and recall.

Results

The trained model achieved an accuracy of X% on the test dataset, with a promising F1 score.

Usage
To predict a class for a new image:

python

def predict_class(path):
    # Your image prediction function here
    
Run the function predict_class('path_to_image') with a retinal image to classify its diabetic retinopathy level.

Dependencies

TensorFlow

Keras

OpenCV

Pandas

NumPy

Matplotlib

License

This project is licensed under the MIT License. See the LICENSE file for details.

