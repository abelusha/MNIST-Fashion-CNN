# MNIST-Fashion-CNN
This a jupyter not book that classifies the MNIST-Fashon dataset. It uses convolutional neuralnetworks (CNN).
The model is sequential model based on keras using tensorflow as a backened.

This is jupyter notebook is adopted from the Original MNIST dataset (the hand wrriten digit image dataset).

The model Hyperparamters are :

batch_size     = 32
nb_classes     = 10
nb_ephochs     = 50
nb_filters     = 32
pool_size      = 2
kernel_size    = 3

Model Architecture :

Layer (type)                 Output Shape              Param #   
=================================================================
conv2d_1 (Conv2D)            (None, 26, 26, 32)        320       
_________________________________________________________________
max_pooling2d_1 (MaxPooling2 (None, 13, 13, 32)        0         
_________________________________________________________________
conv2d_2 (Conv2D)            (None, 11, 11, 32)        9248      
_________________________________________________________________
max_pooling2d_2 (MaxPooling2 (None, 5, 5, 32)          0         
_________________________________________________________________
dropout_1 (Dropout)          (None, 5, 5, 32)          0         
_________________________________________________________________
flatten_1 (Flatten)          (None, 800)               0         
_________________________________________________________________
dense_1 (Dense)              (None, 128)               102528    
_________________________________________________________________
dropout_2 (Dropout)          (None, 128)               0         
_________________________________________________________________
dense_2 (Dense)              (None, 10)                1290      
=================================================================
Total params: 113,386
Trainable params: 113,386
Non-trainable params: 0






