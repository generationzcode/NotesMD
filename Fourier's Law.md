#heat 
## Fouriers Law
* This is for steady or unsteady state heat transfer
* $$\frac{dq}{dA} = -k\frac{\delta T}{\delta n}$$
* q is the heat flow rate across the surface, A is the area of the isothermal surface, k is the conductivity, n is the distance normal to the surface. This relates the temperature gradient to the heat flux
* for steady state:
* $$\frac{q}{A} = -k\frac{dT}{dn}$$
* k, the conductivity is analogous to the viscosity in liquids for momentum transfer
* The thermal conductivity is a weak function of temperature - k=a+bT, usually this doesn't change much

> [!Tip]
> Looking at the above equation with the lens of electricity is really helpful:
> $$-\frac{kA}{\Delta n}*\Delta T = q$$
> Where Delta T can be the potential difference and the preceeding coefficient be -1/R, this to add many different conductivities in series, one simply adds the resistances:
> $$\frac{\Delta T_1+ \Delta T_2}{\frac{\Delta n_1}{k_1A}+\frac{\Delta n_2}{k_2A}} = q$$
> Useful in derivations

## Using Fourier's Law in Cylinders
>[!Attention]
>It's not smart to use the entire laplacian for cylindrical coordinates here, I mean you can, but every component but the radial gets removed and however satisfying that may be, it'll take a while and some people tend to keep getting confused as to what the coordinates mean. Just do it normally. Fight me

$$q = -k*2\pi r L\frac{dT}{dr}$$
=>$$\int^{r_o}_{r_i}\frac{dr}{r} = \int^{T_o}_{T_i}\frac{-2\pi LkdT}{q}$$
=>$$q = \frac{2\pi kL(T_o-T_i)}{ln(r_o/r_i)}$$
Now any normal person would leave it at this, but the law of __comicalicity__ of chemical engineers dictates we make it nearly nausea inducing by introducing an *equivalent area* so we can express the heat transfer across a cylinder or sphere as we would a straight block :/
$$A_L = \frac{2\pi L(r_o-r_i)}{ln(r_o/r_i)}$$

>[!DOne]
>I should do problems from this chapter but it's so easy that I won't.


