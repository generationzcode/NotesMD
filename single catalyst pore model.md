## Wheeler
- chemical reaction on catalyst surface
- one end of the pore is closed
- Diffusion and reaction simultaneously
- ![[Pasted image 20250218095907.png]]
- You can always ignore the surface area which is tiny, real area is from the porous network
- There are a couple of boundary conditions here to define the system
- BC(1) - at x = 0, C_A=C_{AS}
- BC(2) - at x=L,C_A = C_{AL}
- BC(2) - at x=L, \frac{dC_A}{dx} = 0
- This can be understood as a teeny tiny PFR, but instead of taking a differential volume, you take a differential area, by taking differential length - dx
- $$R_a*A = v(C_{A}-C_{AS})$$
- $$\frac{A}{v} = \int^{C_{AL}}_{C_{AS}}\frac{dC_a}{R_a}$$
>[!Warning] The above two equations are incorrect
>The reaction is diffusion controlled (mass transfer controlled)

- Rate = $\frac{\pi d^2}{4}C_{AS}D_A\frac{4k_{sr}}{dD_{Ae}}^{0.5}tanh(L\sqrt{\frac{4k_{sr}}{dD_{Ae}}})$
- The above is found by applying diffusion controlling the reaction instead of kinetics controlling in PFR
- The rate is found by getting the reaction kinetics rate at x=0, because of material balance principles - think about it
- "Hypothetically consider a condition, wherein the complete catalytic surface of the cylindrical pore is exposed to the maximum concentration namely the concentration at the pore mouth - $C_{AS}$, the rate of reaction would be purely kinetically controlled"
- taking the ratio of the two: $$\frac{actual \space rate}{maximum \space rate} = \frac{dD_Atanh(L\sqrt{\frac{4k_{sr}}{dD_{Ae}}})}{2(dD_{Ae})^{0.5}K_{sr}^{0.5}L}$$
- thiele modulus = $$\Phi = L\sqrt{\frac{4k_{sr}}{D_{Ae}d}}$$
- Whats the physical significance of the above? We square it first, since there is a square root in the expression
- $$\Phi^2 = L^2\frac{4k_{sr}}{D_{Ae}d}$$
- The faster the reaction,the higher the modulus, the smaller the pore, the higher the modulus, and so on for every other parameter
- The effectiveness factor of the catalyst pore is $tanh(\Phi)/\Phi$
- As Phi tends to infinity, the effectiveness of the pore tends to 0.
- For the effectiveness factor, we compare the rate of reaction of the entire surface had the same concentration of reactant. This means that this hypothetical surface has a really fast diffusion rate or very slow reaction rate ($k_{sr}/D_{eff}=0$)
- This as we alluded in the previous comment, as $\Phi$ tends to 0, effectiveness factor also tends to 0
- ![[Pasted image 20250221112832.png]]
- ![[Pasted image 20250221112847.png]]
- $$\Phi^2 = L^2\frac{4k_{sr}}{D_{Ae}d} = \frac{k_{sr}C_{AS}\pi d_{pore}L}{\frac{D_{eff}d^2_{pore}C_{AS}\pi}{4L}} = \frac{hypothetical\space maximum\space intrinsic\space Kinetic\space rate}{mass\space transfer\space rate}$$
- So, as we can see phi is the ratio of the maximum possible kinetic rate upon the maximum possible mass transfer across the pore
- $$\eta \Phi^2 = \frac{actual\space rate\space of\space reaction}{mass\space transfer\space rate}$$
## Spherical catalyst pellet diffusion with catalyst
$$C_A = lim_{\alpha R\rightarrow \infty}{C_{AS}\frac{\alpha R}{sinh(\alpha R)}}$$
$C_A = C_{AS}$
$$D_A(\frac{d(C_a\rho_c)}{dr})_r=R$$
> I'll do the derivation latorz

