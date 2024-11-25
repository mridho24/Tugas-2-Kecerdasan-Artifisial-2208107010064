# CNN Model for CIFAR-10 Classification

This project demonstrates how to build and train a Convolutional Neural Network (CNN) to classify images from the CIFAR-10 dataset using TensorFlow and Keras.

## Dataset

The CIFAR-10 dataset contains 60,000 32x32 color images in 10 different classes, with 6,000 images per class. The classes are:

- Airplane
- Automobile
- Bird
- Cat
- Deer
- Dog
- Frog
- Horse
- Ship
- Truck

The dataset is split into a training set of 50,000 images and a test set of 10,000 images.

## Steps Involved

1. **Loading the CIFAR-10 dataset**  
   The dataset is loaded using `tensorflow.keras.datasets.cifar10.load_data()`, which splits it into training and test images along with their corresponding labels.

2. **Data Preprocessing**  
   - The images are normalized to the range [0, 1].
   - The labels are converted into one-hot encoding using `to_categorical`.

3. **Model Architecture**  
   A CNN model is built using the following layers:
   - 3 convolutional layers (Conv2D) with ReLU activation.
   - MaxPooling layers (MaxPooling2D) to downsample the feature maps.
   - A dense fully connected layer with ReLU activation.
   - An output layer with softmax activation to predict one of 10 classes.

4. **Model Training**  
   The model is trained for 10 epochs with a batch size of 64 using the Adam optimizer and categorical crossentropy loss.

5. **Model Evaluation**  
   The training and validation accuracy and loss are plotted to visualize the model's performance.

6. **Model Saving**  
   The trained model is saved in HDF5 format as `cifar10_cnn_model.h5`.

## Requirements

- Python 3.x
- TensorFlow
- Matplotlib

