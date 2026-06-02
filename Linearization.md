>	[!Warning] Requirements
>This note is missing:
>* solved examples
>* multiple variable nonlinear equation
>* A few words on deviation variables
* The process with which we approximate nonlinear systems with linear ones
* Linear systems have closed form, analytic solutions and thus all developmnts toward design of control systems have been limited to linear ones
### Nonlinear equation with one variable
* $$\frac{dx}{dt} = f(x)$$
* to linearize this, simply use a taylor expansion:
* $$f(x) = f(x_0)+\frac{df}{dx}\frac{(x-x_0)^1}{1!}+...$$
* take the first two terms:
* $$f(x) \approx f(x_0)+\frac{df}{dx}(x-x_0)$$
* The error introduced due to this is:
* $$I = \frac{d^2f}{dx^2}\frac{(x-x_0)^2}{2!}$$
## More than one variable
>[!warning] Work in progress
>Will do this later - requires taylor series for multiple variables - need to go over that once
