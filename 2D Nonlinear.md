> finally we get to what we started off trying to understand...
> The "Big Boy" stuff

- General form of a vector field on a phase plane:![[Pasted image 20250906161132.png]]
- cant solve these like we do linear ones since their motion is far more complex and unpredictable
- ![[Pasted image 20250906162838.png]]
- The above phase portrait is of the system:
- $$\dot x = x+e^{-y}$$ $$\dot y = -y$$
## Jacobian
- This follows the logic from before, except the fixed point isn't necessarily 0, so we need to change it about a bit to a account for the eigenvectors to be from the new fixed point
- I am too lazy to latex the equations, so I'll just paste the important parts here
- ![[Pasted image 20250906163442.png]]
- x*,y* are the fixed point coords
- a taylor series expansion of f(x*+u,y*+v) is: ![[Pasted image 20250906163539.png]]
- the first term is 0 and we can ignore the last term for now
- The jacobian matrix:
- ![[Pasted image 20250906163703.png]]
> [!TLDR] What Happened?
> We just linearized the system, then evaluated it like we would a linear system. Since the system will be essentially linear in small intervals, we can assume it to be one. Remember the criteria for attractors and lipunov stability. If a point close to a fixed point tends to come to it or remain close to it, it's stable (lots of catches here but thats the gist of it)
