# Binary-Deep-Image-Classifier
###   A CNN that performs facial recognition image classification using Python, OpenCV, NumPy, Tensorflow, and Keras. 

1.   Convolutional Layers: The model starts with three convolutional layers (Conv2D layers) followed by max-pooling layers (MaxPooling2D). These layers are used for feature extraction from the input image. The convolutional layers have the following characteristics:
        The first convolutional layer has 16 filters of size 3x3, a stride of 1, and uses the ReLU (Rectified Linear Unit) activation function. It takes an input image with dimensions (256, 256, 3).
        The second convolutional layer has 32 filters of size 3x3, a stride of 1, and also uses ReLU activation.
        The third convolutional layer has 16 filters of size 3x3, a stride of 1, and ReLU activation.

2.    Max-Pooling Layers: After each convolutional layer, there is a max-pooling layer (MaxPooling2D) that reduces the spatial dimensions of the feature maps, helping to reduce computational complexity and increase translation invariance.

3.    Flatten Layer: Following the convolutional layers and max-pooling layers, there is a Flatten layer. This layer flattens the 2D feature maps into a 1D vector, which will be used as input for the fully connected (dense) layers.

4.    Dense Layers: There are two dense (fully connected) layers:
        The first dense layer has 256 neurons and uses the ReLU activation function. This layer is responsible for learning complex patterns from the flattened feature maps.
        The second dense layer has 1 neuron and uses the sigmoid activation function. It's a binary classification problem where the network is learning to distinguish between two classes (happy and sad). The sigmoid activation function is appropriate for binary classification as it produces an output between 0 and 1.

Overall, this code defines a CNN for binary image classification (happy vs. sad) using convolutional layers for feature extraction, followed by fully connected layers for making the classification decision. 

