* Measures the probability that a certain sample falls in any one category
* ![[Pasted image 20241112093435.png]]
* The logistic model. We fit B0 and B1 to the data
* A method of maximum likelihood is used to fit the model
* This function will always produce an S shaped curve
* ![[Pasted image 20241112093716.png]]
* the above is the function that is to be maximized to get B0 and B1
>[!Important]
>Dedicate some time to p values and hypothesis testing

* Multiple logistic regressions are also possible, just a small extension of normal logistic regression, however keep in mind that each variable can only have two settings, in other words, it's binomial
* Multinomial logistic regressions solve this - ![[Pasted image 20241112112735.png]]
* this is the normal encoding. If the output has K classes, and p predictors. The regression uses K-1 classes, the Kth class is pretty much implied
* The softmax encoding is the symmetric version of this![[Pasted image 20241112112813.png]]
* This uses all K classes
* Softmax encoding is used a lot in machine learning
