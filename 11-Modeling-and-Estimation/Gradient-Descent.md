# Gradient Descent

### basic idea:
function that can minimize a loss function without forcing the user to predetermine which values of θ to try.

### Intuition:
- we start by picking a θ anywhere we'd like. 
- Then, we iteratively improve the estimate of θ. 
- To improve an estimate of θ, we look at the slope of the loss function at that choice of θ.
  - If slope is negative, increasing θ will decrease the loss.
  - If slope is positive, decreasing θ will decrease the loss.
- The slope of the tangent line tells us which direction to move θ in order to decrease the loss. If the slope is negative, we want θ to move in the positive direction. If the slope is positive, θ should move in the negative direction.


## Summary:

Gradient descent gives us a generic way to minimize a loss function when we cannot solve for the minimizing value of θ analytically.

## Convexity:

- Unfortunately, gradient descent does not always find the globally minimizing θ.
- Luckily, a number of useful loss functions have identical local and global minima. For eg: mean squared error loss function.
- The mean absolute error sometimes has multiple local minima. However, all the local minima produce the globally lowest loss possible.

### Convex functions:
- For some functions, any local minimum is also a global minimum. 
- This set of functions are called convex functions since they curve upward. 
- For a constant model, the MSE, MAE, and Huber loss are all convex.

Formally, a function f is convex if and only if it satisfies the following inequality for all possible function inputs a and b, for all t∈[0,1]:
 ```tf(a)+(1−t)f(b) ≥ f(ta+(1−t)b)```

This inequality states that all lines connecting two points of the function must reside on or above the function itself.
