* [[logistic regression]] is a model where we get the parameters after fitting X to Y, linear discriminant approach is less direct
* Here we model the distribution of the predictors separately for each of the response classes
* Reasons to use this over logistic regression:
* When there is substantial separation between the classes, the parameters for logistic regression are unstable
* If the distribution of the predictors is approximately normal and sample size is small
* This along with a few other techniques, pretty much approximates the probability distribution, to make a bayes classifier. 
* Logistic regression is not bayes classifier because theres no trying to find the probability distribution
## The how
* We assume the probability distribution to be normal
* ![[Pasted image 20241112120116.png]]
* for any one predictor, this is the normal distribution for the Kth class![[Pasted image 20241112120224.png]]
* so the conditional probability of any class given a sample is the above
* ![[Pasted image 20241112120332.png]]
* The bayes boundary line
* ![[Pasted image 20241112122324.png]]
* this discriminant is to be maximized
* the pi_k is approximated to be n_k/n, number of samples that are k vs total number of samples
## More than one predictor
