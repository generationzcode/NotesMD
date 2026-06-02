> This is used in solving differential equations fast. So you convert the differential equation to laplace form and then you do laplace operations like s shifting or t shifting and then you identify the final form to solve it

* It's a very *jugaad* method
* ![[Pasted image 20250108162145.png]]
* this is how you convert a function to laplace form
* it's called the **laplace transform** * gasp *
* The laplace transform converts a function from the time domain to the "s domain". The s domain is something mysterious and ineffable
* an important property of laplace transforms:
* ![[Pasted image 20250206121446.png]]
* laplace transform of derivatives: ![[Pasted image 20250206121609.png]]
* Laplace transform of integrals: ![[Pasted image 20250206121621.png]]
## Frequently used transforms
![[Pasted image 20250206122115.png]]
- [[proofs of some standard laplace transforms]]
## S shift
- Useful property, if we know what the laplace transform of f(t) is, then we can easily get out what the laplace transform of $e^{at}f(t)$ is
- ![[Pasted image 20250206130309.png]]
- where F(s) is the laplace transform of f(t)
## Convolution Theorem
> A convoluted thereom haha
- when two functions are multiplied with each other in laplace form and are to be inverted, we use the convolution theorem: ![[Pasted image 20250206130917.png]]
- This is what convolution is: ![[Pasted image 20250206130935.png]]
- Seems ridiculously complicated
- If the functions f and g are causal (i have no clue what this means but I guess most of them...), then its easier:
- ![[Pasted image 20250206131741.png]]
## Differential equations
- used to solve systems of linear or linear differential equations with constant coefficients
- This is just obvious... 
- Convert the differential equation to laplace form, in the s domain![[Pasted image 20250206133311.png]]
- once you get this, invert the transform back to get T(t)
- Usually, you need to convert this to partial fractions to get the inversion all proper. 
- Inversion is done by identifying standard laplace transforms in the resulting expression
- ![[Pasted image 20250206144328.png]]
## Problems
- [[Laplace transform problems]]