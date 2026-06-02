> Mccabe smith is good for this subject, so is richardson and coulson, treybal too

* Prereqs - Mathematics, material and energy balance, [[Engineering thermodynamics]] and [[Fluid mechanics]]
* "Chemical engineering is a study of a group of industrial processes in which raw materials are converted into useful products"
> [!Example]
> A plant producing phosphoric acid:
> * phosphate rock, H2SO4, in a reactor forming 30% acid, rest gypsum
> * This goes into a crystallizer, then a filtration step - wet product P2O5, lot of gypsum
> * Then a washing step for the dry product, the wash is then recycled into the reactor
> * The wet product goes into the dryer, which then gives us  the product
> ![[Pasted image 20241202112034.png]]

* A unit operation is a basic step in a chemical process that can cause physical changes only
* Adsorption is for gas/liquid solid and absorption is for gas liquid
## Mass transfer
* When a system contains two or more components with different concentrations, there is a natural tendency for a mass to be transferred minimizing the concentration differences.
>[!Important]
>* The transport of one constituent from a region of higher concentration to that of a lower concentration is called as mass transfer
* The difference in concentration (or partial pressure) is the driving force.
### Types of mass transfer
* Diffusive (or molecular) - Occurs in absence of any microscopic motion in the medium. There are two types - molecular and eddy diffusion
* Convective (or forced) - Occurs in presence of motion in the medium
### Ficks law
* Molar flux of species is directly proportional to the concentration gradient in the direction of decreasing concentration
* $$J_{A} = -D_{AB}\frac{dC_B}{dz}$$
* Applicable for molecular diffusion
* Steady state assumption
* The factor is an experimental quantity
# Mass transfer
*  Simple way of solving practical problems related to complex mixing flows and patterns
* mass transfer flux is the rate of mass transfer/area
* $$flux = k_c\Delta C$$
* The typical value of kc for gas phase is 10^(-2) m/s and for liquid phase it's 10^(-5)
### Molar Average Velocity
* $$U = \frac1C\sum{C_iu_i}$$
* Molar flux related to stationary observer:
* $$N_A = C_AU_A$$
* Molar flux related to observer with any velocity
* $$J_A = C_A(U_A-U)$$
* ->$$=C_A-C_A(\frac{C_AU_A+C_BU_B}{C_A+C_B})$$
* $$N_A = (N_A+N_B)(C_A/C)-D_{AB}\frac{dC_a}{dz}$$
* $$N_A = (N_A+N_B)\frac{P_A}{P} - \frac {D_{AB}}{RT}\frac{dP_A}{dz}$$
* We can define two cases here - diffusion of A through non diffusing B, the second case is Gas liquid phase where both are diffusing - equimolar counter diffusion
* So for the first case B is not diffusing and the second has A and B diffusing at the same rates
* N_A is the molar flux of component A, C is total concentration and P is total pressure

>Example
>If Nb =0
> $$N_A(1-C_A/C) = -D_{AB}\frac{dC_A}{dz}$$
> $$N_Adz = -\frac{D_{AB}}{(1-C_A/C)}dC_A$$
> $$N_A*z = C*D_{AB}*(ln((1-C_{A2}/C)/(1-C_{A1}/C))$$

LMCD is the log mean concentration difference which is analogous to the LMTD In [[Heat Transfer]]
## Unit operations
* [[Distillation]] - you distill stuff 
* [[Absorption]] - you absorb stuff 
* [[Filtration]] - you filter stuff 
* [[Sedimentation]] - you sediment stuff 
* [[Drying]] - you dry stuff 
* [[Particle Size Reduction]] - you cut up stuff 