# Notes on Tutorial

## Tutorial 1

The first tutorial is 1_hello_tensorflow.ipynb. It explains the basics of defining the tensors 
(which is just a generalization of arrays, matrices, with a fancier name), and add/multiply/assign operations on them.

> A vector is a 1-d array and is known as a 1st-order tensor. A matrix is a 2-d array and a 2nd-order tensor.

Some key points:

1. Tensorflow works well with numpy package
1. Tensorflow uses delayed computation (compute it only when you explicitly ask it to)

## Tutorial 2

The second tutorial is 2_getting_started.ipynb. It demonstrates how to build a linear regression model using functions
in tensorflow. The key part may be the GradientDescentOptimizer, which makes weight learning really easy.

## Tutorial 3

The third tutorial is 3_mnist_from_scratch.ipynb. It shows how to build a CNN for the MNIST data, including how to download the data, how to parse the data, and how to split the data into training/validation/test sets.

To understand the structure of the CNN model, I find [this video](https://www.youtube.com/watch?v=FmpDIaiMIeA) very helpful. 

There is also another tutorial about building CNN using layers module for MNIST data [here](https://www.tensorflow.org/tutorials/layers). Also take a look.

Now I roughly understand how the model is built, but I cannot run it in Jupyter notebook, because the kernel always dies.
I also cannot run it after converting it to python program because of the same issue. It seems to be caused by too much 
memory usage after researching on the web.

The good news is [this MNIST tutorial](https://www.tensorflow.org/tutorials/layers) works (I can run it).
Will read it next time.
