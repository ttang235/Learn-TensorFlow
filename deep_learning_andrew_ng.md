[youtube video lecture list](https://www.youtube.com/watch?v=7PiK4wtfvbA&list=PLBAGcD3siRDguyYYzhVwZ3tLvOyyG5k6K)

1. Overview
2. What is a neural network
   1. house price example
3. Supervised Learning with Neural Networks
4. Drivers behind the rise of deep learning
   1. deep learning improves with bigger data
5. Binary classification in deep learning
6. Logistic Regression
7. Logistic Regression cost function
8. Gradient Descent
9. Derivatives
10. Derivatives Examples
11. Computation graph
12. Derivatives with a computation graph
13. Logistic Regression Derivatives
14. Gradient Descent on m Training examples
15. Vectorization
    1. prefer vector operation (e.g. numpy.dot(a,b)) to for loops (the former could be 100 times faster)
16. More Vectorization examples
17. Vectorizing logistic regression
18. Vectorizing logistic regression's gradient computation
19. Broadcasting in python
20. Python-Numpy
    1. Use np.random.randn(5,1) or np.random.randn(1,5), instead of np.random.randn(5), because the former ones are matrices,
    while the latter one is a 'rank 1 array' which may have weird behavior.
    1. Use assert(a.shape == (5,1)) to check.
    1. Use a.reshape((5,1)) to make it explicit and the behavior more predictable.
21. Jupyter-ipython
22. Logistic regression cost function explanation
23. neural network overview
24. neural network representation
25. computing a neural network's output
26. vectoring across multiple training examples
27. vectorized implementation explanation
28. Activation Functions
    1. empirically, tanh tends to work better than sigmoid.
    2. ReLU is widely used.
    3. Leaky ReLU is also an option, though not very popular.
    4. In practice, try each of them to see which works best, if possible.
29. Why non-linear activation function?
    - because if you use linear activation function in hidden layer, the combined effect is still a linear transformation,
    which may not be expressive enough (cannot model non-linear relationship between output y and input x)
30. Derivatives of activation functions
    - For both tanh and sigmoid, the derivatives can be expressed in terms of the function value, so it'd be
    convenient to compute them. For y = sigmoid(x), y' = y(1-y); for y = tanh(x), y' = 1-y^2;
31. [continue here](https://www.youtube.com/watch?v=6D0rQxgnrZM&index=31&list=PLBAGcD3siRDguyYYzhVwZ3tLvOyyG5k6K)
