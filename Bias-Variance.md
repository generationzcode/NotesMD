## Bias-variance tradeoff
* the mean squared error in models shows the accuracy 
* It can be shown that it decomposes to:
* ![[Pasted image 20241110130159.png]]
* the bias of the function squared, variance of the function and variance of the irreducible error term
* variance of the function is how much the prediction of some x0 would change if we estimated it on different datasets, same with the error term's variance
* In general, more flexible methods have more more variance. You would see deep learning have a higher variance than linear regression
* bias is the error that is because we're estimating a real life problem. Its the difference between what we got vs whats actually there
* Usually, with more flexible methods, bias initially decreases,hits a hard bottom, then variance starts to increase
* So basically if bias is high, you dont have a model that understands your data at all
* If your variance is high, you've overfit and cant use your model to extrapolate
* Mostly, when the bias decreases, variance increases and vice versa
* The trick is to get both at a low amount
