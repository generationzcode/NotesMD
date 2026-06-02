> a control system for the flow through a pipe...

![[Pasted image 20250401111736.png]]
- assuming there is a fully developed plug flow, the velocity is v and the distance is L, the time taken for the fluid to flow from entry to exit is $$\tau_D = \frac{L}{v}$$
- ![[Pasted image 20250401112047.png]]
- Taking the pipe in the first order system of a tank, we can see that the fluid that enters the pipe at time t is not the fluid that exits the tank at that time. So the fluid exits the pipe at time t+$\tau_D$
- the fluid that exits at time t is y, x is the fluid that enters the pipe at time t:
- $$y(t) = x(t-\tau_D)$$
- $$y(s) = e^{-\tau_Ds}x(s)$$ (due to s shifting)
- so, $$\frac{y(s)}{x(s)} = e^{-\tau_Ds}$$ is the transfer function of the pipe
- We can see how this would affect the control system of the tank. This is the distance dependent lag. Its also the dead time - the time during which we don't know whats going on in the system
- Dead time causes a lot of oscillations and such, so we must reduce it as much as possible
- 