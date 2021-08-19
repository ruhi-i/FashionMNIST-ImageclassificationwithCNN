# FashionMNIST-ImageclassificationwithCNN
Classifying images of clothing articles with Convolutional Neural Networks, using Tensorflow 2

![image](https://user-images.githubusercontent.com/75364712/130087100-1417f633-3f28-4e2a-8677-ca87b585916c.png)

Introduction:

Image Classification is the process of categorizing a group of pixels and assigning appropriate labels to them, based on their characteristics. This is popularly accomplished by Deep Learning Algorithms.

The main objective of this notebook is to classify images of clothing items, using Convolutional Neural Networks(CNN), with a high level of accuracy.
The Dataset

Fashion-MNIST is a dataset of Zalando's article images—consisting of a training set of 60,000 examples and a test set of 10,000 examples. Each example is a 28x28 grayscale image, associated with a label from 10 classes.

Each training and test example is assigned to one of the following labels:

    0 T-shirt/top
    1 Trouser
    2 Pullover
    3 Dress
    4 Coat
    5 Sandal
    6 Shirt
    7 Sneaker
    8 Bag
    9 Ankle boot

Steps taken:

1) Loading the dataset from Tensorflow Datasets, reshaping arrays and checking the shape
2) Visualizing the images with Matplotlib
3) Scaling the inputs
4) Splitting the data into train, validation and test sets
5) Outlining the Model:

   I'm going to build a Sequential Model, and stack the following layers:

    Convolutional Layer: 32 filters of 3x3 size, with ReLU activation function, and initializing normally distributed weights for the filters
    Pooling Layer: 2x2 pool size for downsizing the image
    Dropout Layer: To prevent overfitting the CNN, I'm going to use a dropout rate of 0.2
    Convolutional Layer: 64 filters of 3x3 size, with ReLU activation function
    Pooling Layer: 2x2 pool size for downsizing the image
    Dropout Layer: Dropout rate of 0.2
    Convolutional Layer: 128 filters of 3x3 size, with ReLU activation function
    Dropout Layer: I'm going to use a dropout rate of 0.5 in this layer
    Flattening the input
    Fully connected Layer with ReLU activation
    Output Layer with Softmax Activation
    
 6) Training the Model
 7) Model Evaluation by plotting training & validation accuracy and loss
 8) Testing the Model

Model achieved a Test Accuracy of 91.33% and a Validation Accuracy of 90.62%.
