Date: Dec 19, 2020

Dataset: MNIST and Fashion-MNIST

Method: CNN

Requirements:

In real-world applications, deep learning is complicated by the existence of several important design choices that go into a neural network model. These choices include (but are not limited to):

  • Network architecture. This includes the number of layers, the type of layers, e.g., fully connected, convolutional, pooling, residual connections, etc., and 
    the activation functions.
    
  • Optimization. This includes the optimization algorithm itself, e.g., SGD, Adagrad, Adam, etc., as well as the minibatch size, number of epochs, the learning rate,
    and other hyperparameters.
    
  • Initialization. Common choices include initializing the network weights with independent normal or uniform draws, distributed with a pre-specified mean and variance.
  
  • Regularization. This includes techniques such as dropout, batch normalization, and weight decay, as well as implicit regularization such as early stopping or 
    data augmentation.
    
  • Loss function. For simplicity, we will stick with the standard choices: in our case we will use cross-entropy loss for classification.


These choices can have a substantial impact on the performance of trained neural network models. As a result, it is natural to ask how robust the models are to these design choices. The aim of this project is to investigate how these choices can affect out-of-sample performance and whether good choices for one dataset translate into good choices for another dataset.

Process: 

We first trained an unregularized MLP with 2 hidden layers of 16 hidden units and ReLU activations on the MNIST hand-written digits dataset. Then, we moved to CNN for higher accuracy. We also applied our models to FMNIST to do comparision.
