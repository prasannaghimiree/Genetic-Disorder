# Genetic Disorder Classification using Deep Learning

This project aims to classify genetic disorders from facial images using deep learning techniques. The model identifies the following genetic syndromes:

- **Angelman Syndrome**
- **Apert Syndrome**
- **Charge Syndrome**
- **Down Syndrome**
- **Williams Syndrome**
- **Cannot identify** (if prediction confidence is low)

## Motivation

In countries like Nepal, there are very few genetic doctors, making it challenging to diagnose genetic diseases. This project proposes a deep learning-based model to assist in the early identification of these disorders by analyzing facial features, offering an accessible and reliable tool for both medical professionals and the public. By automating the process of identifying genetic syndromes from facial features, the model aims to help in the early diagnosis and intervention of these disorders, ultimately improving the quality of healthcare in underserved regions.

## Model Overview

The model is based on a Convolutional Neural Network (CNN) architecture designed to recognize facial features that are indicative of specific genetic syndromes. The dataset contains labeled facial images, and the model uses this data to learn the distinguishing characteristics of each syndrome. The architecture is a variation of a simple fully connected network (FirstAttemptFCN), optimized for the task of image classification.

### Model Architecture:
The model is composed of convolutional layers followed by fully connected layers. These layers are designed to extract hierarchical features from the input image, which are then used to make predictions about the genetic disorder present.

## Features

- **Deep Learning Model:** The model utilizes a **FirstAttemptFCN** architecture, which is a fully connected neural network optimized for image classification tasks. The architecture uses a fully connected layer followed by another fully connected layer to output the classification results.
  
- **Data Transformations:** Input images are resized to **256x256** pixels and normalized before being fed into the model for training and inference. The normalization helps to standardize the input data, improving the model's performance and convergence.
  
- **Gradio Interface:** The project includes a simple web-based interface built using Gradio, which allows users to upload images for classification. The interface displays the top 5 predicted genetic disorders along with their confidence scores. This makes it easy for medical professionals or individuals to use the model for diagnosis.

- **Confidence-based Prediction:** If the model's confidence in predicting a disorder is low, it will classify the image as **"Cannot identify"**. This ensures that the model does not provide misleading predictions.


