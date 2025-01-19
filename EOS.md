#thermo 
>[!IMportant]
>$$\frac{H^R}{RT} = Z-1-\frac{A}{Z}$$
>$$\frac{S^R}{R} = ln(Z-B)$$
>$$\frac{U^R}{RT} = -\frac{A}{Z}$$

>[!Example]
>for a steam turbine with input 50 bar, 500 C and 10 bar, 350 C. Steam has a T_c of 647K and Pc of 220.48 bar and Cp of 37.5 J/gmolK

![[Pasted image 20240807101118.png]]

>[!Example]
>Suppose I want to find the latent heat of water @200C, P_sat = 15.538bar. Find it NOW!

![[Pasted image 20240807104503.png]]
## New EOS
We want an EOS that doesn't require Pc, Tc and Vc, so we use a **reduced EOS**
The idea was that at the same "reduced" T and P, T_r and P_r from here on out, all substances would behave the same, they'd have the same compressibility, enthalpy and entropy
T_c is critical temp
>[!Important]
>Reduced Values:
>$$T_r = \frac{T}{T_c}$$
>$$P_r = \frac{P}{P_c}$$
>$$V_r = \frac{V}{V_c}$$


VdW EOS:
$$P = \frac{RT}{V-b}-\frac{a}{V^2}$$
reduced EOS:
$$P_rP_c = \frac{RT_rT_c}{V_rV_c-b}-\frac{a}{V_r^2V_c^2}$$
>[!Principle of Corresponding State]
>Z = f(T_r,P_r,w)
>H_r = f(T_r,P_r)
>S_r = f(T_r,P_r)
r
w is omega and it's a third parameter called accentric factor

## vapour pressure for water
$$log_{10}P^{sat}mmHg = 8.14019-\frac{1810.94}{T\degree{C}+244.485}$$
find $\omega$
>$$\omega = -1-log_{10}P^{sat}_{r}@(T_r = 0.7)$$
>T_c = 647.3K, P_c = 220.5 bar
>T_r= 0.7, T = 453K, T = 179.9C, 
>$$log_{10}P^{sat}mmHg = 8.14-1810/(179.9+244.485) = 7463mmHg = 10 bar = P_r = 0.0453$$
>$$-1-log_{10}0.0453 = 0.344 = \omega$$

[[accentric factor]]

## Using the EOS to get the vapour pressure
Suppose we consider a box with some liquid and some space for it's vapour, to get the p^sat
the system must be at equilibrium. The gibbs energy for this system is:
$$\frac{dG}{dt} = -TS_{gen}$$
This way, dG <= 0
at S_{gen} = 0, dG also =0 and thats when equilibrium happens.
It's when the gibbs energy of the liquid matches the gibb's energy of the vapour


to put this in formulae:
$$G^V = G^L$$
$$G^V-G^{IG} = G^L-G^{IG}$$
$$G^{RV} = G^{RL}$$
$$G^R = H^R-TS^R$$
>[!Important]
>If we consider the gas at low enough pressure, it's ideal and we get the clausius clapeyron equation:
>$$\frac{dlnP^{sat}}{dT} = \frac{\Delta H}{RT^2}$$
>this gives a really interesting comparison for the equation for real gases where the fugacity is actually the vapour pressure of the gas if it was ideal. Cool


$$G^R = \int^{P}_0(V-T\frac{\delta V}{\delta T}_P)dP - T\int^{P}_0(-\frac{\delta V}{\delta T}-R/P)dP$$
$$G^R = \int^P_0(V-RT/P)dP$$
>[!since]
>Vdp = RTln(f)

$$G^R = \int^P_0RTd(ln(f))-\int^P_0RTd(ln(P))$$
$$G^R/RT = ln(f/P)$$
>[!DANGER]
>WHAT IS FUGACITY???  I HAVE NO CLUE. RIGHT NOW ALL WE KNOW IS THAT FUGACITY IS A WAY TO EXPRESS VOLUME IN TERMS OF PRESSURE AND TEMPERATURE BAS ONLY THAT WHAT DOES IT MEAN WHY IS IT SO? SAME WITH ACCENTRIC FACTOR MAN

so when the fugacities are equal, the system is in equilibrium


![[Pasted image 20240808154935.png]]
The fugacity vs pressure for water. The point of intersection is where the vapour pressure is  in equilibrium. This is supposed to be 15.5 bar but I got 54 bar so the VdW equation of state is absolute BS and shouldnt be used by anyone worth their salt why did we learn this I feel cheated I shouldn't have wasted my time on this
## Compressibility factor
* it's the volume of a real gas vs the volume of an ideal gas
* 



> google esoteric

>[!Example]
>Suppose you have a substance with a normal boiling point 56C, TC of 508.1K, PC = 46.9bar, find $\omega$
>Solution:
>So we have the vapour pressure and temperature of the substance at two points. We fit a clausius clapeyron like equation onto this (we cant use the clausius clapeyron equation by itself here because the critical pressure is a little above 0 bar -> 46.9 bar)
>
>$$lnP^{sat} = A+\frac{B}{T}$$
>After fitting, $$lnP^{sat} = 10.893-3579.53/(T)$$
>thus we get omega as 0.3135
>yay

>[!Example]
>Psat at 25C = 23.6mmHg
>Psat at 40C = 55.mmHg
>Find normal boiling point, find latent heat of vaporization
>__Solution__
>same same but differlent
>$$lnP^{sat} = 20.89-5283.76/(273+T)$$
>boiling point - 97.7
>use clausius clapeyron for getting delta H, delta H in clausius clapeyron eqn is latent heat of vaporization and the data points given have a small enough pressure for it to be usable

> VdW gives inaccurate predictions for liquid volume, p_sat and lambda

Now we use omega in our equation of state to make it more accurate
Strongly polar molecules have large omega.
Substances with higher sphericificity have a smaller omega
Noble gases have a small omega and are used as the reference against which the meaning of omega is derived
Omega is of course the accentric factor
## New EOS
$$P = \frac{RT}{V-b}-\frac{a}{V^2}$$
At small volumes and large pressures and smaller volumes, the first term is massive and second not as much and vice versa
* First correction people made is that a and b are not functions of temperature but functions of T_c and P_c and this is obviously wrong. 
* We need a = f(T) and V^2 = f(b)
* People have come up with many different variations
* Redlich-kwong EOS = $$P=\frac{RT}{V-b}-\frac{a}{\sqrt TV(V+B)}$$
* Soave Redlich- Kwong EOS = $$P=\frac{RT}{V-b}-\frac{a(T,\omega)}{V(V+b)}$$
* Peng robinson EOS = $$P=\frac{RT}{V-b}-\frac{a(T,\omega)}{(V+b)^2-cb^2}$$
>[!Todo]
>ask dev where I heard about peng robinson last, it rings a bell...

* These are all semi emprical mostly because of the a
* $$P=\frac{RT}{V-b}-\frac{a(T,\omega)}{(V+b)^2-2b^2}$$
* $$P=\frac{RT}{V-b}-\frac{a(T,\omega)}{V(V+b)+b(V-b)}$$
* The c was rounded off to 2 for aesthetic purposes by peng or robinson probably maybe both
* Patel - Teja EOS
>[!Info]
>DONT MUG THIS UP
>$$b = 0.0778\frac{RT_c}{P_c}$$
>$$a = 0.45724\alpha \frac{R^2T_c^2}{P_c}$$
>$$\sqrt\alpha = 1+K(1-\sqrt T_r)$$
>$$K = 0.37464+1.54226\omega - 0.26992\omega ^2$$
>Now this in Z:
>$$Z^3+(B-1)Z^2+(A-3B^2-2B)Z+(B^2+B^3-AB) = 0$$
>$$A = \frac{aP}{R^2T^2}$$
>$$B = \frac{bP}{RT}$$
>Now if you do all that maths magic you get:
>$$\frac{H^R}{RT} = (Z-1)+\frac{T\frac{da}{dt}-a}{2\sqrt 2bRT}ln(\frac{Z+(1+\sqrt2)B}{Z+(1-\sqrt 2)B})$$




# BIG AWESOME BIG BIG BIG BIG BIG AWESOME
[[Takshil's Problem]]
