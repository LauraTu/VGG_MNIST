## VGG_MNIST
This is a project on MNIST dataset classification using tensorflow with the VGG16 network stucture.

### Network Stucture
+ Resize mnist images to 224\*224
+ 2 64-hidden\_dim convolutional layers
+ 1 maxpooling layer
+ 2 128-hidden\_dim convolutional layers
+ 1 maxpooling layer
+ 3 258-hidden\_dim convolutional layers
+ 1 maxpooling layer
+ 3 512-hidden\_dim convolutional layers
+ 1 maxpooling layer
+ 3 512-hidden\_dim convolutional layers
+ 1 maxpooling layer
+ 1 flatten layer
+ 2 dense layers with dropout
+ 1 logits layer

### Parameters
+ Input_size = [784,], reshape to [28,28]
+ Batch_size = 32
+ Output_size = 10
+ Learning_rate = 1e-3
+ Optimizer = GradientDescentOptimizer
+ Dropout_rate = 0.1
+ Training_size = 55000
+ Validation_size = 5000
+ Testing_size = 10000

### Results
[Epoch 26]

train\_loss=0.000219, train\_acc=0.994785

valid\_loss=0.034767, valid\_acc=0.994828 

test\_loss=0.024464, test\_acc=0.994807