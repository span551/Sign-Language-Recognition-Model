# Sign-Language-Recognition-Model

The aim of this project is to recognize what the person is trying to convey using different hand gestures. The dataset contains 29 classes which comprises of A to Z alphabets, nothing, space and delete hand gestures.

![Image](https://github.com/user-attachments/assets/374f0b08-f4ed-4464-95f3-0f801ee6265b)




 I HAVE USED TWO APPROACHES IN THE ABOVE PROJECT TO ANALYSE THE RESULTS AND COMPARE THEM

 

 (1)Multi Layer Perceptron(MLP) approach




Loading datasets
Defining a function to display sample images from the dataset when their corresponding labels are given as input
Performing Data Augmentation using ImageDataGenerator to import training images and augment more images
Building the Multi Layer Perceptron model
Defining a function to determine the learning_rate decay based on epoch schedule.
Plotting the accuracy and loss curves.

![Image](https://github.com/user-attachments/assets/e2b90f6f-1640-4c4f-9ff3-9fab904b2252)




(2)Convolutional Neural Network(CNN) approach

Loading datasets
Labelling the images before giving it as input to the CNN model
Converting the images and labels into numpy arrays
Generating X data and y data using Image augmentation approac
Visualizing the X data --> sign language image and the y data --> label of the sign language
Data Processing
Performing One Hot Encoding on the categorical features of the training data
Verifying the dimensions of all variables before they are feeded to the models
Building the CNN model
Plotting the accuracy and validation accuracy
Plotting the loss and validation loss
Saving the CNN model
Performing multiclass predictions
Comparing the Actual label vs the Predicted label of the Sign Language image
Confusion Matrix
Classification report of the CNN model


![Image](https://github.com/user-attachments/assets/7dc5986c-5b23-4e4a-8c1e-38626effe504)





LIBRARIES USED

Tensorflow

cv2

glob

matplotlib

random

math

os

numpy

PIL

scikit learn

keras

skimage









MODEL COMPARISON


The MLP model achieved 91.99% training accuracy but suffered from overfitting, with validation accuracy dropping to 68.28%. MLPs are not ideal for image data as they ignore spatial relationships between pixels.

In contrast, the CNN model achieved 99.43% training accuracy and 99.78% validation accuracy, demonstrating superior performance in recognizing American Sign Language images.

Thus, CNN proved to be the optimal approach for this task.










CONCLUSION





In this project we have used a couple of Deep Learning frameworks to recognize the Sign Language. The MLP model performs fairly but gets overfitted. However, CNN approach is used to train the dataset which perfroms well and gives a validation accuracy of 99.78% .





















