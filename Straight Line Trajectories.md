- Two dimensional systems of differential equations have all sorts of trajectories
- One special type of trajectory is a straight line trajectory. When a phase point starting on a particular direction stays in that direction forever, exhibiting simple exponential decay or growth on it
## Linear algebra and eigenvalues
![[Pasted image 20250906152512.png]]
- lets suppose the equation is like the one at the start of [[2D flows]]
- Here $\dot x = A x$
- Anyone can see how if you have an x, which when multiplied with A gives $\lambda x$, you get a straight line trajectory from a fixed point (x=0 is a fixed point for all such systems)
- The terminology for such an x is called an eigenvector and $\lambda$ is an eigenvalue
- ![[Pasted image 20250906152952.png]]
- The above is the solution we are looking for when taking this method
### Finding Eigensolutions
- eigenvalues are given by the characteristic equation $det (A-\lambda I) = 0$
- ![[Pasted image 20250906153143.png]]
- Pretty easy after this. 
- to find the eigenvectors, take v1 and v2 to be the components of the eigenvector. They should satisfy the equation:
- ![[Pasted image 20250906153833.png]]
- From here, it's pretty easy to expand this logic and apply it to the whole jacobian stuff we did in class
>[!FAQ] Why This Works
>- The reason the eigenvalue thing works is demonstrated by the second part - where you use the characteristic equation and show that for an eigenvector to exist, there must be a non trivial solution to Ax = 0. 
>- Now why does a nontrivial solution to Ax = 0 demand a singular matrix? because when you invert something, you are essentially saying there's a one to one relation for that function. For some x, there must be some y. If you have many x pointing to one y, you have something you cant invert - since how do you know WHICH x that y is pointing to?
>- There's also some theory as to how, after finding the straight line trajectories, any linear combination of them gives a general solution to the problem since the eigenvectors are linearly independant, so depending on the initial and boundary conditions, one can infer a particular solution to a set of linear equations
>- All this can be found better documented in kreyzig and I really don't want to get into it

- complex eigenvalues are real head turners
- They occur when the fixed point is the center or a spiral:![[Pasted image 20250906155327.png]]
## Stability
- Yet another picture I have stolen:
- ![[Pasted image 20250906155800.png]]
- $\tau$ is the trace of the matrix and $\Delta$ is the determinant
- But we really don't need to care much for this graph. What we do need to care about is whether the eigen values are both below or above 0
- $\lambda_2<\lambda_1<0$ then we have a stable node
- $\lambda_2<0<\lambda_1$ then we have a saddle point
- $0<\lambda_1<\lambda_2$ then we have an unstable node
