# Stochastic Gradient Descent

## Limitations of Batch Gradient Descent¶

In gradient descent we calculate gradient of the loss function using the average gradient of the loss function using the entire dataset. In other words, each time we update θ we consult all the other points in our dataset as a complete batch. For this reason, the gradient update rule above is often referred to as batch gradient descent.

Unfortunately, we often work with large datasets. Although batch gradient descent will often find an optimal θ in relatively few iterations, each iteration will take a long time to compute if the training set contains many points.
