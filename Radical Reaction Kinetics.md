> All of this is basically useless without experimental validation

A lot of this has been covered in the previous section, I'm just developing it here - getting it all together
### Number Average Degree of Polymerization
* Using kinetics analysis, without taking into account chain transfer:
![[Pasted image 20240913181336.png]]
* Using kinetics analysis, taking into account chain transfer to get the Mayo Walling Equation
![[Pasted image 20240913183908.png]]
$$R_i = 2f[k_d]I$$
k_d is the dissociation constant for the initiator and f is the efficiency factor

- Kinetic chain length is the number average degree of polymerization when radical polymerization goes through steady state kinetics
- When there is a chain growth, the initiation constant - Kd, and all the other chain transfer rate constants are known as velocity constant
- c_m,c_s, c_i are the transfer constants for monomer, solvent and initiator
- $$C_M = \frac{k_{tr.M}}{k_P},C_S = \frac{k_{tr.S}}{k_P},C_I = \frac{k_{tr.I}}{k_P}$$
- $$\bar x_n = v$$(kinetic chain length is v apparently)
- You can substitute I in the equation:
- $$I = \frac{k_tR_p^2}{k_p^2fk_d[M]^2}$$
- $$\frac{1}{\bar x_n} = \frac{k_tR_p}{k_p^2[M]^2}+C_M+C_S\frac{[S]}{[M]}+C_I(\frac{k_tR_p^2}{k_p^2fk_d[M]^3})$$==Under Investigation - fkd or 2fkd==
- $$\bar x_n = \frac{2}{2-\epsilon_{tc}}\frac{R_p}{R_t}$$
- if the termination is by combination, the value of epsilon will be 0, if not then it's 1
- $$Z = 1-\epsilon_{tc}/2$$
- the Z is a factor to multiply the R_t with and R_i with as well
- so $R_i = Zfk_d[I]$
### Diffusion Control
At different conversions, the diffusive properties of the chains differ (lol). This is important because these diffusive properties, control how molecules meet each other and react. Thus if they are low enough in any area they can cause *certain* parts of the radical polymerization mechanism to go slower or faster. Certain parts can be "diffusion controlled"

Types of diffusion
* Segmental Diffusion - Refers to orientation of molecules reacting. Propagation and termination are controlled by this at low conversions since they molecules have to be in correct orientation to react and translational diffusion when the chain is small is good
* Translational Diffusion - Refers to **actual** diffusion (the centre of mass moves). Controls the termination step at high conversions. An interesting effect, known as *autoacceleration* or the *Trommsdorf-Norrish* effect occurs when reaction mixtures become translational diffusion controlled - the termination step decreases and since propagation is not affected by translational diffusion (monomers still diffuse about easily), the conversion increases and the termination step decreases more, so on and so on. The reaction mixture becomes really viscous and even glass like (vitrifies)
* Reactive diffusion - everything slow, chains move only by adding new monomers
### Molar Mass Distribution
[[Molar Mass Distribution]] - when I finally make this page, I'm including this there
![[Pasted image 20240913185147.png]]
Situation is different for combination and Mn/Mw ends up being (2+B)/2

### Determination of Constants
Let some things be mysteries. Why spoil the magic of not knowing the dirty reality of how these constants are found out?
### Temperature
I'm not going into the details - they used the arrhenius equation and they found the dependence of the rate of polymerization and thus degree of polymerization with temperature
$$
\frac{d(ln R_p)}{dT} = \frac{2E_p+E_d-E_t}{2RT^2}
$$
$$\frac{d(ln (X_n)_0)}{dT} = \frac{2E_p-E_d-E_t}{2RT^2}$$
* Ceiling temperature - the temperature at with propagation stops due to the reaction becoming non spontaneous. There's an equation for this, I'll add it later, when they teach us this stuff probably
## Rate constants
- temperature dependant:
- $$K_i = A_ie^{-\frac{E_i}{RT}}$$
- A_i is a factor representing number of collisions and orientation of collisions
- E_i is the activation energy