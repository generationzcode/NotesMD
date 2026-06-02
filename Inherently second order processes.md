* Fluid or solid mechanic processes possessing inertia and subjected to some acceleration
## Pneumatically operated valve
* forces: force exerted by compressed air, force exerted by the spring, frictional force due to contact of the stem
* ![[Pasted image 20250121113121.png]]
* engineering drawing of a pneumatic valve - drawn to specs
* the force balance gives:
* $$M\frac{d^2x(t)}{dt^2} = p(t)A-Kx(t)-C\frac{dx(t)}{dt}$$
* rearranging:(copy later)
* say $\tau^2 = \frac{M}{K}$; $2\epsilon\tau = \frac{C}{K}$;$K_p = \frac{A}{K}$ 
* you have now: $$\tau^2\frac{d^2x}{dt^2}+2\epsilon\tau\frac{dx}{dt}+x=K_pp$$
* The above is the standard form of dynamic equation for a second order system
* Taking laplace transform,
* $$\tau^2[s^2x(s)-sx(0)-x'(0)]+2\epsilon\tau[sx(s)-x(0)]+x(s) = K_pp(s)$$
* $$(\tau^2s^2+2\epsilon\tau s+1)x(s) = K_pp(s)$$
* $$\frac{x(s)}{p(s)} = \frac{K_p}{\tau^2s^2+2\epsilon\tau s+1}$$
* $$\frac{x(s)}{p(s)} = \frac{\frac{A}{K}}{\frac{M}{K}s^2+\frac{C}{K}s+1} = G_p(s)$$
* for the control valve, usually M << K and hence the dynamics of this system can be approximated to be that of first order dynamics
* $$G_p(s) = \frac{\frac{A}{K}}{\frac{C}{K}s+1} = \frac{K_v}{\tau_vS+1}$$
* In terms of deviation from the steady state value: $$\frac{\bar{x(s)}}{\bar{p(s)}} = \frac{K_p}{\tau^2s^2+\epsilon\tau s+1}$$ $$s = \frac{-2\epsilon\tau+\sqrt{4\epsilon\tau^2-4\tau^2}}{2\tau^2} = \frac{\epsilon\frac{+}{}\sqrt{\epsilon^2}}{\tau}$$
* We now take the case of a unit step chance in p(s),i.e. p(s)=1/s $$\bar{x(s)} = \frac{K_p/\tau^2}{s(s-s_a)(s-s_b)} = \frac{K_p}{\tau^2}(\frac{A}{s}+\frac{B}{s-s_a}+\frac{C}{s-s_b})$$
* where s_a and s_b are the roots of the quadratic equation
* $$s_a = $$
### Critically damped response
* $\epsilon = 1$
* 