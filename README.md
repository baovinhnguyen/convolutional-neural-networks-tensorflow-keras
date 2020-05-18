# Convolutional-Neural-Networks-with-TensorFlow-and-Keras

The objective of this project is to classify 10 classes of images, including cats, dogs, frogs, airplanes, and automobiles. 
The data set that I used is CIFAR-10, consisting 60,000 images, equally divided among 10 classes. First, I followed a standard tutorial (http://tinyurl.com/cifar10-exercise). However, the method following the tutorial only gets approximately 80% accuracy. 

Therefore, I adjusted the model in different ways: changing elements of the model (change strides from 3x3 to 5x5), cut first 2 CONV layers and 1 POOL layer, add 2 more CONV layers with feature size 16 each, and add more epochs.
The second method that I used is to do data augmentation. I flipped all images horizontally then added into the training data set. Doing that way, I doubled the training data set without needed to collect more data.
The result is that the second method (data augmentation) earns better accuracy compared with the first method (adjust the model). 

