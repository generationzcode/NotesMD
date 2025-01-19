#thermo 
> Related to [[Real Gases]]

* Since we know, from experiment, that the equilibrium of a single component single phase system is controlled by only two state variables, we can express any other variable as the function of these two variables in the following manner:
* $$dU=(\frac{\delta U}{\delta T})_VdT+(\frac{\delta U}{\delta V})_TdV$$
* This is like taking a substance from one state to the other by keeping one variable constant, then changing the other, then doing the other way round
* 
* This can be better understood from linear algebra, when there are two independent variables and a bunch of dependent variables. A thermodynamic system is the same. We can look at it like a vector space
* 
* For open systems, a sizing parameter like number of moles can also be added to the mix
* 
* An interesting nature of the partial derivatives shown above is that they depend on the path you take. dU/dT at constant volume is not the same as taking it at constant pressure. This is because moving it along the constant pressure line will give a different value as well, making the total the same. Also the final state itself is different if you just change the temperature at constant pressure vs constant volume, so you're really comparing apples to oranges
* 
>[!important]
>A few important things:
>![[Pasted image 20241104110814.png]]
>* Similar to what I said above, ![[Pasted image 20241104112848.png]]
>* ![[Pasted image 20241104112905.png]]
>* ![[Pasted image 20241104112919.png]]
>* This is the triple product rule, If X increases with Y (holding Z constant), and Z increases with X (holding Y constant), then Y must decrease with Z (holding X constant) to keep the overall relationship consistent
>* This also shows how he movement of x is dependent on the movements of y and z


We need a section for [[Vector Calculus]]
## Maxwell relations
* We need to express variables like entropy and internal energy in terms of variables we can measure, such as pressure or temperature. To do this, we use the maxwell relations
* we shall try and get to them
* for open systems: $$dU = TdS-PdV+GdN$$
* $$dU = TdS-PdV = \frac{\delta U}{\delta S}_VdS+\frac{\delta U}{\delta V}_SdV$$
* $$\frac{\delta U}{\delta S}_V = T, \frac{\delta U}{\delta V}_S = -P$$
* from these two, a list of more relations can be derived. They aren't really derived as much as they are identified:
* If we know the equation for any differential variable in the system expressed in two other variables, the components multiplied on it, will be equal to the partial derivative of the variable with respect to the independent variable keeping the other independent variable constant
* These are not as difficult as I initially thought...
* These aren't maxwell relations though, those are slightly more:
* So in general, to get those, you differentiate the identities above by the *other* independent variable, for both independent variables, and those are equal to each other
* ![[Pasted image 20241104153905.png]]
* [[EOS]] and the preceeding notecovers equation of state pretty well. There's peng robinson, van der waals. You could look at the algebraic manipulations to get to the roots and all but honestly, its not worth it. 
## Corresponding states
* This got me somewhat confused in class
* So basically, we got reduced pressure, reduced temperature and reduced volume - P/P_c, T/T_c, V/V_c, where c means critical point.
* The principle of corresponding states says that any van der waals fluid (not **any** fluid), that has the same reduced pressure and reduced temperature will have the same reduced volume and is thus in a corresponding state. Why they couldn't just define Tc, Pc in each equation and leave pressure and temperature alone is beyond me... Maybe they just wanted to be elegant
* Accentric factor is used in some equations of states to account for non sphericity
## Functional group contribution estimation 
* The first assumption confirms that I should be an engineer because I knew it before even reading about it :lol:
* Each functional group contributes the same properties regardless of presence of other functional groups or structure of molecules.
* The above is almost **never** true in real life (or ideally for that matter)
* This assumption could be improved to include effects of first or second level neighbours, ==I'm pretty sure I could come up with something to fit.==
* The joback method (jugaad method more like):
* ![[Pasted image 20241104195013.png]]
* subscripts c,b and f are critical, boiling and freezing point, respectively
* an example of the functional group parameters
* ![[Pasted image 20241104195112.png]]
* If you use this and cause an explosion that injures yourself and/or others, I am not liable
## Speed of sound
* I only include this because I remember spending days and nights trying to figure it out myself without success back in the ol' days
* YKW, Forget it. I'll do this later. Other work calls me