When you have two or more random variables
>[!Danger]
>brace yourself
flashbacks of multivariable calculus incoming
 
Most of the stuff on conditional probability, marginal distributions are so painfully obvious that i think its insulting for you, dear reader, for me to write on it. If you found these notes, you're probably smart enough to know that.

Totally not because I'm lazy

## Independence 
you call two random variables independent when their occurrence or non occurrence doesn't affect the other's contribution to probability. For example -  
* **number of taco bell tacos eaten** and **number of difficult visits to the washroom** are ==dependent== random variables, but 
* **number of taco bell tacos eaten** and **number of leaves fallen from the tree** in front of me are ==independent== random variables
there are a bunch of conditions for this:
* The probability at any point is the multiplication of the marginal probabilities at that point
* the marginal probability is equal to the conditional probability for both variables

## Covariance
* Get the mean values from the marginal distribution and: cov(X,Y) = E[(X-MEAN)(Y-MEAN)] = E[XY]-mean_y*mean_x
* the covariance looks like variability but it isn't, it's just a measure or linear relationship between variables
* The covariance may or may not be expanded to more than 2 variables, from what I've seen on the internet, its still kinda
* the correlation coefficient is just covariance/sqrt(variability of x* variability of y)
## Bivariate distribution
just normal distribution with two random variables

## Problems
### Question 1
A small company is to decide what investments to use for cash generated from operations. Each investment has a mean and standard deviation associated with a percentage gain. The first security has a mean percentage gain of 5% with a standard deviation of 2% and the second security provides the same 5% percentage gain with a standard deviation of 4%. The securities have a correlation of -0.5. If the company invests 1 million dollars in each security, whats the mean and standard deviation of the return?
![[Pasted image 20240910132751.png]]