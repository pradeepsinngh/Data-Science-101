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

Gradient descent gives us a generic way to minimize a loss function when we cannot solve for the minimizing value of θ analytically. As our models and loss functions increase in complexity, we will turn to gradient descent as our tool of choice to fit models.
