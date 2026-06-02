> It's just a linear regression with an activation function (heaviside step function)

- The perceptron finds a hyperplane that separates the data items
- Perceptrons can solve binary classifications for linearly separable instance spaces
- XOR- the great enemy
- I don't know why I made this as a separate note. As awesome as it is, it doesnt deserve a separate page
- $$W_{ij+1} = W_{ij}+\alpha*(T_j-Y_j)*X_{ij}$$
- The above is the learning equation (a modified delta learning method with the transfer function 1 since it's linear)
- ![[Pasted image 20250320092444.png]]
- Here, theta is the threshold, when it is above the threshold it's 1, otherwise it's 0
- Perceptrons can also have an extra X_0 which is always 1, with a weight that can be changed, this allows the bias also to be learned. Here then, the threshold will be 0
>[!Todo]
>Think about *why* such a gradient descent delta learning method actually works in optimizing parameters

