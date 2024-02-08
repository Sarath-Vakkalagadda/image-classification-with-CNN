# image-classification-with-CNN

This project focuses on classifying images of dogs and cats using a Convolutional Neural Network (CNN) implemented with the Keras library. The dataset used in this project is sourced from Kaggle. The CNN model is designed to recognize and distinguish between images of dogs and cats.

# Requirements
TensorFlow
Keras
Matplotlib (for visualization)
Pandas (for data manipulation)

Dataset is taken from kaggle - https://www.kaggle.com/datasets/salader/dogs-vs-cats

# CNN Architecture
The model consists of three convolutional layers with increasing filter sizes (32, 64, 128).
Each convolutional layer uses a 3x3 kernel for feature extraction.
Rectified Linear Unit (ReLU) activation functions are applied to introduce non-linearity.
Batch normalization is applied after each convolutional layer to normalize the activations, improving convergence and training stability.
MaxPooling layers follow each convolutional layer, reducing the spatial dimensions of the feature maps.
A 2x2 pooling window with a stride of 2 is used to downsample the feature maps.
MaxPooling layers follow each convolutional layer, reducing the spatial dimensions of the feature maps.
A 2x2 pooling window with a stride of 2 is used to downsample the feature maps.
The flattened output is fed into two fully connected (dense) layers with 128 and 64 neurons, respectively.
Rectified Linear Unit (ReLU) activation functions are applied to these dense layers.
Dropout with a rate of 0.1 is used to reduce overfitting by randomly dropping a fraction of the neurons during training.
The final dense layer with a single neuron and a sigmoid activation function is used for binary classification (dog or cat).
The sigmoid activation function outputs a probability indicating the likelihood of the input image belonging to the positive class (cat).
