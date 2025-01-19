#thermo 
![[Pasted image 20240911105458.png]]
![[Pasted image 20240926122107.png]]
suppose we mix 3kg of water and 1kg of pure H2SO4 at 21.1 C adiabatically, what will the final temperature be?
![[Pasted image 20240911110600.png]]
> [!Info]
> if we actually did this isothermally, we'd have to remove energy since the total enthalpy of the mixture reduces. This is because of hydrogen bonding formed between h2so4 and h20

$$\Delta_{mix}H = H-\sum x_iHi$$
* The above equation can be used for any of the variables like gibbs free energy, entropy, etc
## Redlich Kister expansion
* This is a polynomial fitted for delta H mix
* $$x_1x_2[A+B(x_1-x_2)+C(x_1-x_2)^2+...]$$
* x1 and x2 are the mole fractions of the two components
>[!Todo]
>Fit a redlich kister expansion to H2SO4

## Why are we doing this?
* One of the things that separates chemical engineers from the rest of humanity is that we are able to separate stuff.
* Distillation, crystallization, liquid liquid extraction, etc.
* So we'll have a mixture and a process which outputs a number of pure components
* Now if we want to know the minimum work or heat required to separate something, we can use this
## Equilibrium
* Imagine we have a phase equilibrium between a liquid and it's vapour:
* ![[Pasted image 20240925112145.png]]
* I don't know why you should imagine this I just copied this off the board
* ![[Pasted image 20240925113256.png]]
* The above can be written for vapour as well
* the derivative of G with respect to components in the mixture is called the chemical potential of that particular component in whichever phase it's in
* ![[Pasted image 20240925114057.png]]This is also called the partial molar gibbs energy
* ![[Pasted image 20240925114641.png]]
* An interesting derivation later we see that at equilibrium, the chemical potential of each component in the liquid phase must be equal to the chemical potential of that component in the vapour phase
## Relationship between $\Delta_{mix} G$ and partial molar gibbs energy, and other partial molar quantities with their Del mix values
![[Pasted image 20240925121402.png]]
* Last year we had learnt that enthalpy is the addition of enthalpy multiplied by the mole fraction of each component, THIS WAS WRONG
* It's the partial molar enthalpy of a component multiplied by it's mole fraction and added up with all the other components - thats the actual enthalpy
* Gibbs duhem - get familiar
## Partial molar characteristics
![[Pasted image 20240926110930.png]]
Now, using the Redlich Kister expansion
![[Pasted image 20240926111833.png]]
## Special case: Mixture of ideal gases
* N number of ideal gases are being mixed at a certain temperature 
* Volume change due to mixing is 0, $$\Delta_{mix}V = 0$$
* ![[Pasted image 20240926115354.png]]
* This means that the partial molar volume is equal to the volume of the pure substance
* ![[Pasted image 20240926115840.png]]
* ![[Pasted image 20240926120504.png]]
* ![[Pasted image 20240926120640.png]]
>[!Problem]
>Suppose we have an isothermal separation like:
>![[Pasted image 20240926120951.png]]

>[!Solution]
>![[Pasted image 20240926121734.png]]

## Condition for Equilibrium
* The Partial Molar gibbs free energy of all components has to be the same
>[!Problem]
>A problem from the green envelope

![[Pasted image 20241003114806.png]]
Bdababsoia eiasid
The del mix when x tends to 0 also ends up tending to 0
>[!todo]
I need to study sandler later today after the graph theory and all ka kaam

>[!Danger]
>Another problem. I am so hungry I don't think I can solve it I shouldn't have skipped breakfast

* Non ideal mixture - $$\Delta_{mix}M-\Delta_{mix}M^{IM} = M^{ex}$$
* Mex is the excess property of a real gas
>[!Important]
> A reminder for why we are doing all this - we are doing this to get to raoults law, henry's law and solubility

* $$H^{ex} = \Delta_{mix}H-0=\Delta_{mix}H$$
* $$V^{ex} = \Delta_{mix}V-0=\Delta_{mix}V$$
* $$U^{ex} = \Delta_{mix}U-0=\Delta_{mix}U$$
* You might notice a pattern here, but that's because you are stupid and actually for quantities like entropy and gibbs free energy and the sort, there is another term after the delta mix to get the excess
### Another way to write excess properties
* $$M^{ex} = (M-\sum{x_iM_i})-(M^{IM}-\Delta{x_iM_i})$$
* $$M^{ex} = M-M^{IM}$$
* Now, using summability relation
* $$M^{ex} = \sum{x_i\bar{M_i}}-\sum{x_i\bar{M_i}^{IM}}$$
* $$M^{ex} = \sum{x_i(\bar{M_i}-\bar{M_i}^{IM})}$$
* Now if we want the **partial molar excess property** (what a mouthful) at constant temperature, pressure and other components' moles:
* $$\bar{M_i}^{ex} = \frac{\delta {(n^tM^{ex})}}{\delta n_i}$$
* Now wat dis look lyk?
* $$\bar{M_i}^{ex} = \bar{M_i}-\bar{M_i}^{IM}$$
* $$\bar{H_i}^{ex} = \bar{H_i}-H_i$$
## Messing around with residuals
* $$G^R = G-G^{IG} = \int_0^P{(V-V^IG)dP} = RTln(f/P)$$
* The above is for one component. The below is for multiple components
* $$\bar{G_i}-\bar{G_i}^{IGM} = \int_0^P(\bar{V_i}-V_i)dP = RTln(\frac{\bar{f_i}}{P_{y_i}})$$
* The f_i bar is the fugacity of the component in the mixture, NOT the partial molar fugacity
* Pyi is the partial pressure of the gas
* $$\bar{G_i}^{ex} = (\bar{G_i}-\bar{G_i}^{IGM})-(\bar{G_i}^{IM}-\bar{G_i}^{IGM})$$
* $$\bar{G_i}^{ex} = RTln{\frac{\bar{f_i}}{P_{y_i}}}-(G_i+RTlny_i-(G_i^{IG}+RTlny_i))$$
* =>$$RTln{\frac{\bar{f_i}}{P}}-[G-G^{IG}]$$
* $$G^{exv} = RTln{\frac{\bar{f_i}}{y_if_i}}$$
* $$G^{exl} = RTln{\frac{\bar{f_i}}{x_if_i}}$$
## A little further?
At equilibrium:
$$\bar{G_i}^V = \bar{G_i}^L$$
$$\bar{G_i}^{exv}+\bar{G_i}^{IM} = \bar{G_i}^{exl}+\bar{G_i}^{IM} $$
$$RTln{\frac{\bar{f_i}^V}{y_if_i}}+G_i+RTln{y_i} = RTln{\frac{\bar{f_i}^L}{x_if_i}}+G_i+RTln{x_i}$$
$$\bar{f_i}^V = \bar{f_i}^L$$
$$\bar{f_i} = y_if_i$$
the above only works for ideal mixtures - like the fi bar related to the pure component fugacity

for the non ideal condition:
$$\bar{f_i}^L = a_if_i^L$$
the a_i is the activity coefficient
>[!Quote]
>If Prathamesh were normal, his activity coefficient would be 1/88, but since he interacts with 7 people in the class at any point in time, his activity coefficient is 7/88

$$\bar{f_i} = (\tau_ix_i)f_i^L$$
for vapour phase, IM:
$$y_if_i^V = \tau_ix_if_i^L$$
$$y_i\phi_i*P = \tau x_i f_i ^L$$
phi is the fugacity coefficient, which is the ratio of fugacity to the actual pressure
$$y_i\phi_i*P = \tau x_i f_i^{sat}exp(\frac{V^L(P-P^{sat})}{RT})$$
since the vapour phase is an IM, it's pressure is low enough and the pressure is equal to the fugacity
$$Py_i = \tau_ix_i(P_i^{sat}\phi _i^{sat})$$
the exponent to e is small enough for that part of the equation to be equal to 1
If liquid phase is also an ideal mixture then, 
$$Py_i = x_iP_i^sat$$
Dis is raoults law
>[!Danger]
>WHAAAA. THIS IS SO OBVIOUS WHY DID WE SPEND LIKE 5 CLASSES PROVING IT? AND NOW WE HAVE A TEST. I HATE THIS LIFE I HATE EVERYTHING AND NOW PROF SAID THAT WE WILL NEVER USE IT

# WE DIDNT HAVE A TEST. WHAT IS THIS THIS IS TEXTBOOK MANIPULATION. MY FEELINGS ARENT A PLAYTHING DAMMIT

![[Pasted image 20241009115411.png]]
![[Pasted image 20241009115634.png]]
* So now all we do is get the enthalpies of all the streams and we assume the mixing process is at steady state. The difference between the in and out enthalpies give you the heat you need to remove from the process
* So just mass balance and energy balance
* This is below our level
* No calculation will be done!

## Problems
* 