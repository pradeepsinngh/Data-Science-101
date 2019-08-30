# Stochastic Gradient Descent

## Limitations of Batch Gradient Descent:

In gradient descent we calculate gradient of the loss function using the average gradient of the loss function using the entire dataset. In other words, each time we update θ we consult all the other points in our dataset as a complete batch. For this reason, the gradient update rule above is often referred to as batch gradient descent.

Unfortunately, we often work with large datasets. Although batch gradient descent will often find an optimal θ in relatively few iterations, each iteration will take a long time to compute if the training set contains many points.


## Stochastic Gradient Descent:

To circumvent the difficulty of computing a gradient across the entire training set, stochastic gradient descent approximates the overall gradient using a single randomly chosen data point. Since the observation is chosen randomly, we expect that using the gradient at each individual observation will eventually converge to the same parameters as batch gradient descent.

**Note** that choosing the points randomly is critical to the success of stochastic gradient descent! 

We most commonly run stochastic gradient descent by shuffling the data points and using each one in its shuffled order until one complete pass through the training data is completed. If the algorithm hasn't converged, we reshuffle the points and run another pass through the data. Each iteration of stochastic gradient descent looks at one data point; each complete pass through the data is called an epoch.


## Behavior of Stochastic Gradient Descent

1. Since stochastic descent only examines a single data point a time, it will likely update θ less accurately than a update from batch gradient descent. 

2. However, since stochastic gradient descent computes updates much faster than batch gradient descent, stochastic gradient descent can make significant progress towards the optimal θ by the time batch gradient descent finishes a single update.

## Way Ahead: Mini-batch Gradient Descent
Mini-batch gradient descent strikes a balance between batch gradient descent and stochastic gradient descent by increasing the number of observations that we select at each iteration. In mini-batch gradient descent, we use a few data points for each gradient update instead of a single point.
