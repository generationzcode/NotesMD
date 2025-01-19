## Equivalent Diameter
* As chemical engineers, we assume everything is a circular cross section in a pipe. When in reality it is not, we use equivalent diameter to get it's cross sectional area
* Equivalent diameter is defined as:
* $$4*\frac{cross\space sectional\space area}{wetted\space perimeter}$$
> [!Odd Exercise in Proving the Obvious]
> Prove that the equivalent diameter of a circular cross sectional area of a pipe with diameter d is d

### Solution 
* $$\frac{4*\pi *d^2}{4*\pi d} = d$$
* Thus proven :Cry: :fart: :vomit:
* Why did I have to do this useless proof
### For square of side l
$$\frac{4*l^2}{4*l} = d = l$$
### For equilateral triangle of side l
$$4*\frac{\sqrt{3}l^2}{4*3*l} = d = \frac{l}{\sqrt3}$$
### For limpet coils (half circle)
$$\frac{4*\pi d^2}{8*d*(1+\pi/2)} = D_{eq} = \frac{\pi d}{2+\pi}$$
>Home assignment - find equivalent diameter for polygon of n sides, equilateral. (n>=3)
 
> This equivalent diameter is used to calculate reynolds number for a non circular cross section pipe 

> Note - Don't be an idiot when making calculations. Thickness of a pipe is $(D_2-D_1)/2$
> if D1 is the inner diameter and D2is the other diameter

> [!reynolds number calculation]
> D = 0.7m, V = 42m/s, $\rho = 1000$, $\mu = 11*10^{-3}Pa*s$

> (0.7)(42)(1000)/(0.011) = $2.6*10^6$

velocity taken in calculation is the average velocity in the pipe $v_{av}$