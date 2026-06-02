and then failing to intersect. This is exactly the scenario in the prototypical- Lets take this system of equations:
- ![[Pasted image 20250906131958.png]]
- we can represent them in a matrix form:![[Pasted image 20250906132028.png]]
- **$\dot x = Ax$**
- It's very easy to get fixed points to such a system by solving the linear system. But we don't care much for linear systems so lets ignore that
## Stability
- ![[Pasted image 20250906142924.png]]
- all the black points here are stable points since they're attractors (except d)
- A point is said to be attracting if all trajectories that start near it approach it as $t\rightarrow \infty$
> [!Important] Saddle Points and Manifolds
> -  the phase plane (e) shows a saddle point. 
> - It's y axis is it's stable manifold. The stable manifold is the set of initial conditions such that as $t\rightarrow \infty$, the phase point approaches the fixed point.
> - The x axis is the unstable manifold. As $t \rightarrow -\infty$, the phase point approaches the fixed point
- A point is said to be lipunov stable if any trajectory starting close to it remains close to it. 
- Using this definition, a non attracting point like in (d) is lipunov stable (neutrally stable)
>[!Danger] Mind Blown
>![[Pasted image 20250906145859.png]]
>Fixed point that is not lipunov stable but attracting. All trajectories that start near it approach it as $t\rightarrow \infty$, but don't **remain close to it** as $t\rightarrow \infty$

