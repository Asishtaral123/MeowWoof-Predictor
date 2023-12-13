# MeowWoof-Predictor
# Convolutional Neural Network (CNN) for Image Classification

This repository contains code for building and training a CNN using TensorFlow and Keras for image classification, specifically distinguishing between cats and dogs. The code also includes a section for making a single prediction.

## Contents

1. Data Preprocessing:
   - Training set and test set are generated using `ImageDataGenerator` to perform real-time data augmentation.
   - Images are rescaled, sheared, zoomed, flipped horizontally, rotated, and shifted both in width and height.
   - The training set contains 8000 images belonging to 2 classes, while the test set contains 2000 images.

2. Building the CNN:
   - A Sequential model is initialized using TensorFlow and Keras.
   - The CNN architecture consists of:
     - Convolutional layer with 32 filters, a 3x3 kernel, and ReLU activation.
     - Max pooling layer with a pool size of 2x2 and strides of 2.
     - A second convolutional layer and max pooling layer for feature extraction.
     - Flattening layer to convert the 2D feature maps to a 1D vector.
     - Fully connected layer with 128 units and ReLU activation.
     - Output layer with 1 unit and sigmoid activation for binary classification.

3. Compiling and Training the CNN:
   - The model is compiled using the Adam optimizer and binary crossentropy loss.
   - Training is performed on the training set, and evaluation is done on the test set over 25 epochs.

4. Making a Single Prediction:
   - An example of making a prediction on a single image is included.
   - An image is loaded, preprocessed, and passed through the trained CNN to predict whether it's a cat or a dog.



 Run the Code:
   - Open the Jupyter notebook or Python script containing the code.
   - Execute the code cells or run the script.

 Make Predictions:
   - Replace the example image in the "single_prediction" folder with your own image.
   - Run the prediction code to classify the image as a cat or a dog.

Feel free to explore and modify the code for your specific use case or dataset. Contributions and improvements are welcome!

Note: Ensure that you have TensorFlow, Keras, and other required libraries installed before running the code. You can install them using the provided `requirements.txt` file.
