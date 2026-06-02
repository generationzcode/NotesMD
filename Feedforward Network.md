> builds from [[Artificial Neural Networks]]

- Most of the essentials are the same, derivative of transfer function used in the gradient descent function, etc.
- ![[Pasted image 20250320105147.png]]
- For the bias, we use the same logic as in [[Perceptron]], just make another variable thats always 1 and vary the weight
- The activation functions are also known as transfer functions or squashing functions
- Activation functions must be continuously differentiable, monotonic, smooth
- Vanishing gradient - Problem faced by gradient descent methods. The gradient of the error at times becomes really small, causing changes to be made to the weights to also be small. 
- Gradient descent uses $1/2*(T_j-Y_j)^2$ as the error (uses MSE only, just 1/2 is used here to simplify derivations)
- I'm too lazy to cover all of backprop here, just the most important part - use delta learning algorithm, except the T-Y part is "propagated" through the layers by multiplying it by the weight at the edge. This makes sense because the weight kinda determines how much that node affected the error, so it the weight is smaller, it didn't affect the error nearly as much (scaled to the input as well) and so the change to the weight in that node will be negligible
- Bucket brigade system uses a backprop analogous system to allocate rewards or punishment to a RL system that determines how much fitness value to allocate to particular gene rule in the fitness function
- Radial basis function input does no computation and the second to third layer there is a non linear mapping to a higher dimension where patterns emerge (similar to support vector machines)
- Autencoders do unsupervised learning by encoding and decoding the same thing to reduce dimensionality for a set of data
