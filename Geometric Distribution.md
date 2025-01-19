This is related to the binomial distribution, but instead of the random variable being number of successes, the random variable is number of trials to get one success

The geometric distribution gives us information of how many trials are needed until a success is obtained - it gives the probability

mean - 1/p
variance - $$\frac{(1-p)}{p^2}$$
theres also a lack of memory property but thats so obvious I don't want to mention it here its just insultingly obvious

the negative binomial distribution is a generalization of the geometric distribution where the random variable is changed from number of trials to get r successes

since out of r successes, r-1 successes can be placed anywhere in the sequence of n-1 trials our of n trials,
$$P(X=n) = C^{x-1}_{r-1}*(p)^r(1-p)^{n-r}$$
mean - r/p
variance - $$r\frac{1-p}{p^2}$$
## Problems
### Question 1
A player of a videogame fights opponents until he loses, after which he stops playing. The probability of winning against an opponent is 80%. What is the expected number of game plays till a player contests four or more opponents
![[Pasted image 20240910110141.png]]
