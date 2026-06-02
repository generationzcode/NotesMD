

- extended from [[Equation of motion]]
## Equation of Continuity
![[Pasted image 20250708090445.png]]
- What go'eth in, go'eth out as long as what be'eth in doesn't over be'eth in
- In cylindrical coordinates:
- $$\frac{\delta (\rho r v_r)}{r\delta r}+\frac{1}{r\delta \theta}(\rho v_\theta)+\frac{\delta}{\delta z}(\rho v_z)$$
- The diagram is in my notebook. Request for it physically if you want.
- it starts something like:
- $$[\rho rd\theta dzdr]_t^{t+dt} + [\rho*v_rrdzd\theta]^{r+dr}_{r}+[\rho*v_\theta dzdr]^{\theta+d\theta}_{r}+[\rho*v_zrdrd\theta]^{z+dz}_{z}$$
- then we divide the whole thing by the control volume, do some calculus formality and we have what was written on the board
- Again, the diagram is in my notebook
## Getting the Velocity Profile
> How we'll do this without the momentum transfer equations, I am unclear

- $v_r$, $v_\theta$ = 0
- These are laminar flow conditions
- No slip condition, the velocity of the fluid at the boundary of the annulus is the same as the velocity of the boundary
- Momentum transfer equations:
### $r$ Component
- $$\rho(\frac{\delta v_r}{\delta t}+v_r\frac{\delta v_r}{\delta r}+\frac{v_\theta \delta v_r}{r\delta \theta} - \frac{v_\theta^2}{r}+v_z\frac{\delta v_r}{\delta z}) = -\frac{\delta P}{\delta r} + \mu(\frac{\delta}{\delta r}(\frac{\delta(rv_r)}{r\delta r})+\frac{\delta^2v_r}{r^2\delta \theta^2}-\frac{2\delta v_\theta}{r^2\delta \theta}+\frac{\delta^2 v_r}{\delta z^2})+\rho g_r$$
- now we pick out what doesn't exist and make a simpler eqn:
- $$0 = 0$$
- wow.
- I guess we aren't using that equation then.
- There *are* other components' equations
>[!quote] Arjun, note this down
>advantage of cartesian, its a symmetrical system
### $\theta$ component
- $$\rho(\frac{\delta v_\theta}{\delta t}+v_r\frac{\delta v_\theta}{\delta r}+\frac{v_\theta \delta v_\theta}{r\delta \theta} - \frac{v_rv_\theta}{r}+v_z\frac{\delta v_\theta}{\delta z}) = -\frac{\delta P}{r\delta \theta} + \mu(\frac{\delta}{\delta r}(\frac{\delta(rv_\theta)}{r\delta r})+\frac{\delta^2v_\theta}{r^2\delta \theta^2}-\frac{2\delta v_r}{r^2\delta \theta}+\frac{\delta^2 v_\theta}{\delta z^2})+\rho g_\theta$$
- Again, the whole thing is just $$0=0$$
### $z$ component
- Now we do the only component that yields anything useful
- $$\rho(\frac{\delta v_z}{\delta t}+v_r\frac{\delta v_z}{\delta r}+\frac{v_\theta \delta v_z}{r\delta \theta} - \frac{v_zv_z}{\delta z}) = -\frac{\delta P}{\delta z} + \mu(\frac{\delta}{r\delta r}(\frac{r\delta(v_z)}{\delta r})+\frac{\delta^2v_z}{r^2\delta \theta^2}-\frac{\delta^2 v_z}{\delta z^2})+\rho g_z$$
- Now, when we filter this out:
- $$0 = -\frac{\delta P}{\delta z} + \mu(\frac{\delta}{r\delta r}(\frac{r\delta(v_z)}{\delta r}))+\rho g_z$$
- This note is lagging my computer, so we'll continue on the next one for the profile