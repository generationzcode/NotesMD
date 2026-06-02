> from SNARC to deepthink R1

- There are a bunch of nodes and a bunch of connections, each connection has a weight, bias and activation function (to non-linearize the signal)
- The signal enters from the input layer, undergoes multiplication with the weight and addition of the bias, after which it goes through an activation layer, which either lets it through or doesnt, it does this through many hidden layers before it's finally revealed at the output layer
- This was inspired by neurons and such

## Weights and Biases
- These are the parameters of the model
- ![[Pasted image 20250318151959.png]]
- There is the sigmoid activation, ReLU activation and many others
- negation of bias is the threshold
- ![[Pasted image 20250318152115.png]]
- ReLU -> Rectified linear unit
## Learning
- This is done through backpropagation, which I'll write about in a bit
- This is basically an optimization process
- Done through perceptron learning rule, delta learning rule and backpropagation
- These processes use an error estimate called the mean squared error, which is just the mean of the squared error (This cannot be misinterpreted)
## History
- McCullock and Pitts make a "nerve net", basically made logic units with thresholds, excitory inputs and inhibitory inputs, where inhibitory inputs have absolute veto power over the excitory inputs and all the excitory inputs have the same weights, which then go through a transfer function with a fixed threshold to give the output
- Hebbian learning - a neuroscientific theory, not a maths thing. "cells that fire together wire together"
- SNARC - the first neural analog computer
## Sub symbolic vs symbolic
- Neural nets are a good example of sub symbolic AI, so here we'll cover the differences between the two and the similarities in learning and representation
- Symbolic AI uses logic, functional and object oriented representations 
- Learning mechanisms are external to symbolic AI, whereas in sub symbolic, its at the core of the method
- The learned concepts are very explicit and readable in symbolic as compared to sub symbolic AI
- Symbolic systems are reshaped and redefined by new learning as compared to sub symbolic, which doesn't change it's architecture on learning new ideas
