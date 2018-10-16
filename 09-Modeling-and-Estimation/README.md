# Modeling and Estimation

### What is a model?
- A model is an idealized representation of a system. 
- For eg, if we drop a steel ball off the Leaning Tower of Pisa, a simple model of gravity states that we expect the ball to drop to the ground, accelerating at the rate of 9.8 m/s². This model also allows us to predict how long it will take the ball to hit the ground using the laws of projectile motion.

### NOTE:
How do we choose a model? 
How do we know whether we need a more complicated model?

### Loss Function:
A loss function is a mathematical function that takes in an estimate θ and the points in our dataset y1,y2,…,yn. It outputs a single number, the loss, that measures how well θ fits our data. 

In mathematical notation, we want to create the function:
```L(θ,y1,y2,…,yn)= …```

- The loss function outputs lower values for preferable values of θ and larger values for worse values of θ. 
- Always select the value of θ that produces a lower loss than all other choices of θ — the θ that minimizes the loss. 

### Mean Squared Error:
- We would like our choice of θ to fall close to the points in our dataset. 
- Thus, we can define a loss function that outputs a larger value as θ gets further away from the points in the dataset. 
- We start with a simple loss function called the mean squared error. 

Here's the idea:
- We select a value of θ.
- For each value in our dataset, take the squared difference between the value and theta: (yi−θ)^2
  - Squaring the difference in a simple way to convert negative differences into positive ones. We want to do this because if our point yi=14, θ=10 and θ=18 are equally far away from the point and are thus equally "bad".
- To compute the final loss, take the average of each of the individual squared differences.
