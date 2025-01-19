>[!TLDR]
>Making a temperature profile dance

#heat 
>I need kreyzig because I don't want to remember variable separable solution of differential equations. Honestly I like them solved numerically but an analytic understanding of the world is sometimes fun. forget it, solve this yourself.

* Why is it unsteady? - because the temperature profile changes with time until it becomes linear
* Why won't a linear temperature profile change with time? - Take a really thin slice of a slab with a Delta T temperature difference. The heat flux across this slab will no doubt be dependant on Delta T divided by the thickness of the slab. Now take every slab before it, if the Delta T is the same across the same thickness in every single slab -> the heat flux will be the same, no heat gets left over, no heat gets snatched away. The temperature profile is unaffected. 
* I know the above isn't really a proof because it is dependent on itself but it's a neat explanation
* So in a nonlinear profile, the delta T/ delta x will change with x as:
* $$\frac{\delta T}{\delta x}_{x+dx} = \frac{\delta T}{\delta x}_x+\frac{\delta}{\delta x}\frac{\delta T}{\delta x}\delta x$$
* thus the heat flow out of the thin slab layer is:
* $$-kA(\frac{\delta T}{\delta x}_x+\frac{\delta}{\delta x}\frac{\delta T}{\delta x}\delta x)dt = q$$
* and the heat accumulated:
* $$-kA\frac{\delta T}{\delta x}dt+kA(\frac{\delta T}{\delta x}_x+\frac{\delta}{\delta x}\frac{\delta T}{\delta x}\delta x)dt = kA\frac{\delta^2T}{\delta x^2}dxdt$$
* this can be equated to:
* $$\frac{\delta T}{\delta t}\rho C_pAdxdt =  kA\frac{\delta^2T}{\delta x^2}dxdt$$
* $$\frac{\delta T}{\delta t} = \frac{k}{\rho C_p}\frac{\delta^2T}{\delta x^2} =  \alpha \frac{\delta^2T}{\delta x^2}$$
* This alpha is called the *thermal diffusivity* of a material
* Solve this, don't solve this no one really cares ig
## Effective Coefficient
> We haven't done this in class so don't you worry you stupid little

* What I understood of this is basically you gotta take the average bulk temperature as the temperature of the substance thats in unsteady state and pretend that's it's steady state temperature.
* Times have changed and we don't need such jugaad but heres the example they gave for spherical particles
* feelin lazy