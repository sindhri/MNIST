# MNIST digit recognition
Use 28x28 pixel images to recognize digit 0-9  
Credit: Deep Learning with Python by Jason Brownlee  
![MNIST](https://github.com/sindhri/MNIST/blob/master/doc/img1.png)

## baseline MLP
![MLP](https://github.com/sindhri/MNIST/blob/master/doc/img2.png)  
flattern and normalize the input  
MLP with two dense layers  
categorical cross entropy as the loss function, adam as the optimizer, and accuracy as the metrics.  
10 epochs with batch size = 200  
Baseline Error: 1.67%

## simple CNN
![CNN](https://github.com/sindhri/MNIST/blob/master/doc/img3.png)  
reshape and normalize the input  
simple CNN with 1 convolutional layer, 1 pooling, 1 dropout, 1 flattern, 2 dense layers  
Much slower than MLP  
categorical cross entropy as the loss function, adam as the optimizer, and accuracy as the metrics.  
10 epochs with batch size = 200  
CNN Error: 1.09% reduced error rate

## larger CNN
![CNN2](https://github.com/sindhri/MNIST/blob/master/doc/img4.png)  
larger CNN with 2 convolutional+pooling layers, 1 dropout, 1 flattern, 3 dense layers
Much slower than MLP  
categorical cross entropy as the loss function, adam as the optimizer, and accuracy as the metrics.  
10 epochs with batch size = 200  
Large CNN Error: 0.77%, improved!
