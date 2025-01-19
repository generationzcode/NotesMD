>[!Info]
>People from a hundred years ago tried to express deviation from ideality using compressibility factor
#thermo 

We will try to write the compressibility factor z as a polynomial, also known as the virial equation of state:
$$Z = 1+\frac B{V}+\frac C{V^2}+...$$
This can also be expressed as a function of pressue:
$$Z  =1 + B'P+C'P^2+...$$
B,C,B',C' are all functions of temperature
At normal temperatures, B and C will be negative. This is because Z at lower temperatures and pressures are mostly below 1

* To find B',C' experimentally, we can take a limit as such:
* $$lim_{P->0}((Z-1)/P) = B'+C'P$$ This is essentially the derivative of compression factor and since P is 0, everything else disappears
* Most of the time we use the virial equation to get the values at areas near ideality, for other conditions we use the PrEOS. In the virial equation we mostly use the first coefficient
## Getting a relation between B and B' and C and C'
* $$P = \frac {RT}{V}+\frac{RTB}{V^2}+...$$
* Substituting this in the compressibility equation in terms of pressure, we get:
* $$B' = \frac B {RT}$$
* $$C' = \frac{C-B^2}{R^2T^2}$$
* so we all decided that c is useless and we got:
* $$Z = 1+\frac{BP}{RT}$$
* $$V = RT/P+B$$
* B is a function of temperature by the way
### Getting the residual values
$$H^R = \int^P_0(V-T\frac{\delta P}{\delta T})dP$$
$$BP-PT\frac{dB}{dT}$$
ok now the residual entropy
$$S^R = \int^P_0(\frac{\delta V}{\delta P}-R/P)dP$$
$$-P\frac{dB}{dT}$$
Gr is just BP LOL

## B
How we get the B? HOW
Half a century after all creation,people gave B as a function of temperature and accentric factor
$$\frac{BP_C}{RT_C} = B^0+\omega B'$$
$$B^0 = 0.083-0.422/T_R^{1.66}$$
$$B' = 0.134 - 0.172/T_R^{4.2}$$
>[!Bug]
>Steam turbine operating between 50 bar and 10 bar, 500 C and 350 C, find S_gen and W_s

## Solution 
Obviously I'm not solving this,I'll tell me how though...

work shaft is just delta H, you can get delta H by getting the residual enthalpies at the two states and the ideal enthalpies at the two states and getting the difference

S_gen is just delta entropy using residual entropy and the ideal entropies at the two state and yay

the real kicker in the question is probably just finding out the derivative of B with respect to temperature
