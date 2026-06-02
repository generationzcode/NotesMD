> Someday I will cover linear algebra in my notes. Someday.

- The example they gave in the book is of $\dot x = \sin x$, so we'll go with that
- ![[Pasted image 20250905211616.png]]
- This is the solution to the above differential equation. It reads pretty badly and you can't get a lot of information out of it. So we try to look at it geometrically
- ![[Pasted image 20250905211707.png]]
- If we consider the equation to be speaking about the velocity of a particle, we can interpret the above graph as how the velocity of the particle changes with x
- If we consider the equation to be speaking about the velocity of fluid flowing with respect to x, things get a little more interesting
- The points where $\dot x = 0$ are called **fixed points**. This is where there is no flow.
- There are certain fixed points to which fluid flows to (arrows on either side point to it), these are called attractors or sinks. They are stable fixed points
- Fixed points from which fluid flows away from are unstable and called repellers or sources
## Stability
- reason we call attractors stable is because if you move something away from it, based on the first derivative, it should come back
- A good method to go about finding these points is to imagine a particle called a phase point at some x_0 and see how it moves along the x axis, along a trajectory. 
- The trajectory represents the solution of the differential equation.
- ![[Pasted image 20250905222148.png]]
- This is a phase portrait
- This, by the way is the same phase portrait we would plot in [[Instrumentation and process control]] 
While this isn't really a great coverage of how a differential equation can be looked at as a vector field (a lot of the technical stuff is skipped), it seems like a good physical understanding