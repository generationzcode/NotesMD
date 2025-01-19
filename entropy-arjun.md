#thermo 
> Related to [[Entropy]]

The requirement for this arises from linear algebra, of all things... 
* We have the mass balance, energy balance equations. These two are used to solve for two variables, which determine all the other variables in a state. Sometimes, these two equations aren't enough to determine the equilibrium conditions, here, a third equation, entropy balance is used - this is for a single phase, isolated system, multiphase is covered later
* Also, the first two equations don't say much about what "can or cant" happen - they do, but there's still another constraint we need. A rock could instantly lower it's temperature and jump up by itself, and that would be alright if we just looked at energy and mass balances. This is why we need entropy balance.
* In essence, we have nothing to describe equilibrium, and it's state in a system. Mass and energy balance are OK with any state as long as those two aren't violated.

> Entropy is a state function. In a system in which there are flows of heat by conduction and flow of work across system boundaries, the conductive heat flow and not the work flow, causes a change in entropy of a system; This rate of change in entropy is Q/T where Q is the rate of heat conducted and T is the temperature. If in addition, there are mass flows at the boundaries, the total entropy will also change due to this convected flow. That is, each element of mass entering or leaving the system carries with it it's entropy

$$\frac{dS}{dt} = \sum^K_{k=1}\dot{M_k}{S_k}+\frac{\dot{Q}}{T}+\dot{S}_{gen}$$
The equation, S, on the left hand side is the total entropy, while S on the right hand side (not S_gen), is the entropy per unit mass(couldnt figure out how to use carets in latex). S_gen is the entropy generated in the system due to inefficiencies, and must always be equal to or above 0

* S_gen is the entropy created in a system, since this always must be above or equal to 0, the presence of it causes irreversibility. Irreversibility in the sense that the system is now forever different to what it was a moment ago, we can never turn back the clock and reduce entropy because S_gen can never be below 0. So unless it is equal to 0 all the time, the system will never go back to what it used to be. 

> [!IMportant]
>  Something funny that NO ONE says in class - all irreversibility can be traced back to conduction - viscous conduction. Even movement due to a finite pressure difference is irreversible purely because of viscous conduction due to friction. :/ This makes entropy so much easier to understand - its ALL heat conduction

![[Pasted image 20241103164321.png]]

* Interesting consequence - reversible processes extracting work from the system to give to the surroundings, maximum work is done for a given change of state of the system (because so little energy is lost to conduction), the processes giving work to the system for a change of state require the least amount of work for it
* [[Gibbs Energy Arjun]]

## Refrigeration 
* This is a cycle - you got the condenser, the evaporator, the nozzle and the compressor. The compressor puts work in the system, makes the fluid high pressure, liquid. The nozzle causes isentropic (not really) expansion, condenser releases heat to the surroundings, evaporator absorbs heat from the cooled substance. 
* The trick to refrigeration which I wasn't able to get in [[Entropy]], is that the heat put in from the cold side and the heat released into the hot side isnt the same, the heat in the hot side is the cold side+ work shaft
## Problems
* Couldn't be bothered :coolglasses:
* I'm doing the illustrations from sandler.