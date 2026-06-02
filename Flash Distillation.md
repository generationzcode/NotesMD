
## Treybal, BK dutta
 >Treybal and BK dutta do it this way
 
 ![[Pasted image 20241223115909.png]]
* flash distillation drum
* the relative volatilities need to be very far apart from each other
* the drum is kept at a low pressure
* this is also called equilibrium distillation
* ![[Pasted image 20241223120728.png]]
* ![[Pasted image 20241223120904.png]]

> A liquid mixture containing 50 mole% each of benzene and toluene at 40C is to be continuously flash vapourized to vaporize 60 mole % of the feed. The residual liquid product contains 35% mole benzene. The enthalpies per mole of feed, the liquid product and the vapor product are 2,5 and 30 kJ/mole, respectively. Calculate the heat added per kJ per mole of the vapor product

## McCabe smith
- ![[Pasted image 20250202161655.png]]
- a is the feed pump, b is the heater, c is the valve to lower the pressure of the fluid before entering d, the flash distillation drum, where it is given enough time in intimate mixture to make sure the vapor and liquid are in equilibrium in the drum
- if f is the mole fraction of the feed that is vaporized,$$x_F = fy_D+(1-f)x_B$$ is the component balance of feed
- $$f=\frac{D}{D+W}$$
- in the above equation, we have two unknowns, to solve, we use the x-y equilibrium curve and find the intersection for x_B and y_D:$$y = -\frac{1-f}{f}x+\frac{x_F}{f}$$ against the 
- at x_F, y is also x_F, so on the x=y line, when this intersects, you get (x_F,x_F)
- ![[Pasted image 20250202171816.png]]
## Why
>[!warning] Unstable Info
I've decided to add this section to notes from now on (especially ones with conflicting info like this), since I've found most people don't care about this aspect of engineering as its all application, so just learn how people said we should solve problems and don't question it. 
While there's nothing much wrong with that, I don't think that kind of thinking will survive reasoning models like O3. To create new things, solve unsolved problems, we need to understand the source code - the fundamentals and the "whys". I've been wasting a good bit of time to find the "whys" behind mostly everything I'm learning but I am afraid a lot of others aren't. In any case, it'll sharpen my thinking

- if you look closely at the mccabe smith solution, it's a lot like an operating line ([[Stage processes#Operating line diagram]]). This is because it is an operating line - what are operating lines but component balances graphed out? It does differ from an operating line on two counts it seems - (1) it's constrained to one point, (2) it doesn't have anything to do with [[constant molal overflow]]. ==this opinion is in it's infancy, it's mostly stupid==
- How are the two methods similar? the treybal and bk dutta method is solving the same problem, but instead of f, it's using (related but not same) W/D. The same algebraic form is used, just caught from another end
## Problems
- [[Problems on flash distillation]]