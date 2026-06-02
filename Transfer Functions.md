> This is a method of providing a direct relationship between inputs and outputs.

## Why?
> Mostly I end with why, but this time I think I should start with it

- It's simple, easy to evaluate
- How else could we accomplish the same thing? We would model the process separately for each different type of input - something like a convolution
## Process with single output
![[Pasted image 20250206142917.png]]
- suppose the output, y, depends on the input, f(t) through the nth order differential equation:
- ![[Pasted image 20250206143119.png]]
- converting y and f to deviation variables from y=0,t=0, taking laplace transform of both sides:
- ![[Pasted image 20250206144235.png]]

- G(s) is called a transfer function and to get the output of a system, you simply multiply the input with it in laplace form and then invert the resulting expression to t domain to get the output in terms of time
- With a process containing more than one input, you get something like: ![[Pasted image 20250206145112.png]]
- which then can be shortened to : ![[Pasted image 20250206145134.png]]

The following is a diagram of this scenario
![[Pasted image 20250206145206.png]]
- transfer function = laplace transform of the output function in deviation form/laplace transform of the input function in deviation form
## Multiple Inputs Multiple Outputs
- Lets go with the example in stephanopoulos
- ![[Pasted image 20250206145926.png]]
- two inputs - f1, f2, outputs first order linear differential equation
- initial conditions are y1,y2 =0 at t=0
- ![[Pasted image 20250206150103.png]]
- converting everything to deviation variables (easy since it's all 0 at the start so anything at all is deviation) laplace transforming the above equations: ![[Pasted image 20250206150214.png]]
