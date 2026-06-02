>I'd like to write something on the momentum flux tensor - most of it I can understand, just the viscosity terms normal to the planes are tough to get. These can be quickly and easily summarized as the effects of stretching

- ![[Pasted image 20251026134954.png]]
- Now viscous stress we can figure out from [[Newtons Law of Viscosity]], to get the molecular stress, one must take into account the pressure:
- $\pi_{ij} = p\delta_{ij}+\tau_ij$
- $\delta_{ij}$ is called the kronecker delta and is 1 for xx,yy,zz and such and 0 for all other components
>[!Warning] Take Note!
>Getting stresses from velocity gradients isn't as easy as we make it seem in [[Newtons Law of Viscosity]], BECAUSE in that page, we use an elementary flow (just in one direction) so our $tau_{yx}$ is simply $-\mu\frac{\delta v_x}{\delta y}$
>
>When you have velocity in all sorts of directions, you get some really unintuitive looking results based on a couple of assumptions

- So how do we get the viscous stresses from velocity gradients?
- There's a bunch of rules, but only one is really any important - all the viscous stresses need to be symmetric. $\tau_{ij} = \tau_{ji}$
- Why? Because when we have viscous forces, we know that the fluid cant be in pure rotation (no slippage). Suppose xy and yx are not the same. There would be some rotation of the fluid. And since it's made up of molecules, the molecules, at their tiny size would be rotating because of it. This ends up imparting a near or actually infinite angular momentum - which isn't possible
- Of course, you could ask - how does the molecule know this is impossible and stop it from happening and ensure symmetry? That's a valid question and to understand really whats going on, we need a molecular picture of viscosity, which I'd like not to delve into (because I don't know much about it)
- So, on applying this rule, we get:
- $$\tau_{ij} = A(\frac{\delta v_{j}}{\delta x_i}+\frac{\delta v_i}{\delta x_j})+B(\frac{\delta v_x}{\delta x}+\frac{\delta v_y}{\delta y}+\frac{\delta v_z}{\delta z})\delta_{ij}$$
>[!FAQ] Doubt
>- The first term is understandable - it's symmetric, but the second is only nonzero when you have a normal term - which is anyways not required to be "symmetric". So why is it defined as such?
>- What's really great is that I won't write anything about this point here. B is 0 for incompressible flow anyways and that's all we'll care about. Enjoy having this sit in your mind over the years collecting dust until you're 70 and retired.

- A becomes $\mu$ since on relating it with the elementary example in our previous page, we know that $\tau_{yx} = -\mu \frac{\delta v_x}{\delta y}$
- 