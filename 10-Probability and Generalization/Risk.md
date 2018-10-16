# Risk

A model's risk is the expected value of the model's loss on randomly chosen points from the population.

- Unlike loss alone, using risk allows us to reason about the model's accuracy on the population in general. 
- If our model achieves a low risk, our model will make accurate predictions on points from the population in the long term. 
- On the other hand, if our model has a high risk it will in general perform poorly on data from the population.

- the model's risk is the bias of the model plus the variance of the quantity we are trying to predict:
R(θ)=bias+variance

Thus, the risk is minimized when our model has no bias.

## Analysis of Risk:
Notice that when our model has no bias, the risk is usually a positive quantity. This implies that even an optimal model will have prediction error. Intuitively, this occurs because a constant model will only predict a single number while X may take on any value from the population. The variance term captures the magnitude of the error. A low variance means that X will likely take a value close to θ, whereas a high variance means that X is more likely to take on a value far from θ.
