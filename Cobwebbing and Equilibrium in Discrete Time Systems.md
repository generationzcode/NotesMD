- Continuous systems have fixed points when their first order derivatives equal to 0. Their stability is judged by a concept called lyapunov stability, which we discuss
- For discrete time systems, the equilibria occur similarly:$$N_{t+1} = N_t$$
## Cobwebbing
- These are diagrams that show the movement of a discrete time system. 
- the x axis is $N_t$, the y axis is $N_{t+1}$
- Two lines are drawn. One is y=x ($N_{t+1}=N_t$), the other is the actual curve of $N_{t+1}$ vs $N_t$
- ![[Pasted image 20251107160854.png]]
>[!FAQ] The real question
>Why do we use cobweb analyses in our discrete time systems? 
>They are really good to visualise fixed points.  A normal plot of N_t vs time will give you maybe a fixed point and even that can move an any time, we don't now. A cobweb diagram. through the curve, when it intersects the equilibrium line - it shows you exactly where the equilibrium is, whether it is one or not and whether it is unstable of stable. Might be rambling though, a pretty girl is sitting near me

## Stable??
- Take a discrete time equation: $$N_{t+1} = f(N_t)$$
- So the equilibrium point is: $$N^* = f(N^*)$$
- IS IT STABLE?
- I'm not deriving the lyapunov stability stuff but, generally:
- $$|\frac{df(N)}{dN}|<1$$ means it's stable.
- Imagine a cobweb diagram schewpit
## Periodic stability
- This was painfully obvious stuff I could never come up with
- ![[Pasted image 20251107171611.png]]
- This is what we define f^n as
- If we have a 2 cycle, n becomes 2, so after f and another f, we get N_0 again. Cool
- So how do we know this 2 cycle is stable? Absolute comedy
- $$|\frac{df^n(N)}{dN}|<1$$
- :shocked face:
If a periodic point is stable, the entire orbit is stable.