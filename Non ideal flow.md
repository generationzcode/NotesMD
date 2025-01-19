> Difficult but rewarding

While we can describe reactors as ideal plug flow, ideal backmix or ideal batch reactors, in reality, none of the reactors at large scale follow these equations well. This is due to short circuiting and recycling of fluid

## Residence Time Distribution
> Great idea in general but how does an RTD have anything to do with non ideal flows in reactors???

* $\theta = T/t$, theta is simply the dimensionless time in terms of spacetime of the reactor
* The internal age distribution of the contents of the reactor is denoted by I
* ![[Pasted image 20240621004336.png]]
* Exit age distribution is a distribution of residence times of fluid in the reactor
## Determining internal and exit age distributions
* These are all done using stimulus response techniques, where we add a stimulus in the reactor and see how the system responds to it
### F curve
* When a step tracer is added to the reactor
* ![[Pasted image 20240621202105.png]]
* It slowly increases from 0 to one
$$
F = C/C_{0}
$$$$F + I = 1$$$$F = \int_{0}^{\theta}{E(\theta)d\theta}$$
### C curve
![[Pasted image 20240621202300.png]]
* This happens when a pulse input is added. It forms a "C" shaped curve
* $C=E$
* $$C=E=\frac{df}{d\theta}=-\frac{dI}{d\theta}$$
To get the conversion, simply get the conversion as a function for spacetime and integrate it over the distribution

## The Dispersion Model
* ![[Pasted image 20240621225105.png]]
* This is for packed bed and tubular reactors (plug flow basically)
* The idea here is that there is diffusive mass transfer that occurs between any slice of fluid in the plug flow and the rest of the fluid axially in front and behind it
* Fick's law of diffusion:$$\frac{dC}{dt}=D\frac{d^2C}{dt^2}$$
* Peclet number measures the intensity of dispersion, with it being 0 for ideal plug flow and infinity for ideal backmix $\frac{D}{\mu L}$ 
* The C or F curve can be converted to a theoretical curve by fitting to the data and the relationship between standard deviation, mean of $\theta$ and D/uL is given by a set of equations found by **Levenspiel the greatest human** himself around page 266 of his stellar book, Chemical Reaction Engineering
* This kind of data analysis to get peclet number is usually done using a pulse tracer input. A pulse input manytimes causes flow disturbances at it's point of entry and to correct for this, readings are taken at two downstream points and the delta of the two points is taken for standard deviations and all
* The formulae for getting the peclet number from these deltas are also given in levenspiel
* When they give bed porosity and such, its to calculate the space time of the reactor so we can get the dimensionless units which are used to get peclet number and all
* The first part is accounting for bulk flow, The second for diffusive mass transfer and third for reactive dissapearance![[Pasted image 20240621235412.png]]![[Pasted image 20240621235423.png]]
* ![[Pasted image 20240621235442.png]]
* These three equations are the same and are used to find conversions for a dispersed plug flow reactor
## Tanks in series
> It is time to congratulate ourselves as we have survived the first wave of a non ideal world
> pat yourself on the back. * *pats* * 
* If we hit ourselves in a head a bit hard, really batter the skull, we realize that the dispersion model is actually really hard and we can easily model some amount of axial mixing using a number of backmix reactors.
* ![[Pasted image 20240622173336.png]]
* The above are the equations for number of backmix reactors, j
## Mixed flow
* When either model isnt enough to describe a reactor, a model made up of many different kinds of flow patterns is called a mixed model
* there are plug flow regions, dispersed plug flow regions, backmix regions, deadwater regions
* Bypass flow - when a portion of liquid bypasses the vessel or a particular flow region
* Recycle flow - when a portion of fluid leaving a flow region is recycled back into in
* Cross flow - when there is exchange between flow regions but no net transfer of liquid
* ![[Pasted image 20240622184349.png]]
* The above is what the mean theta should look like if there is no deadwater region
* 