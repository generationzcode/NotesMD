* At the point of incipient fluidisation, equations for packed bed flow are applicable.
* Take a look at the carman kozeny equation and the packed bed equation
* $$V_{ave} = \frac{\epsilon^3}{180(1-\epsilon)^2}(\frac{(1-\epsilon)(\rho_P-\rho)L_{Tube}gd_P^2}{\mu L_{tube}})$$
* This was derived after substituting the delta P from fluidization in the carman kozeny equation
* $$v_{ave} = \frac{\epsilon^3(\rho_P-\rho)gd_P^2}{180\mu (1-\epsilon)}$$
* A value of 3.36 rather than 5 for the carman kozeny constant is used - it matches the experimental data better
* minimum fluidisation velocity is given by: $$v_{mf} = \frac{\epsilon_{mf}^3(\rho_P-\rho)gd_P^2}{180\mu (1-\epsilon_{mf})}$$
* the value of epsilon mf is a function of the size distribution, shape and surface properties of the particles - its the voidage lol
* for turbulent flow, use the ergun equation:
* $$\frac{\Delta P}{L_{tube}} = 150\frac{(1-\epsilon)^2\mu v_{avg}}{\epsilon ^3 d_p^2}+1.75\frac{(1-\epsilon)\rho v^2_{avg}}{\epsilon ^3d_p}$$
* dp = diameter of the sphere having the same V/S ratio as the actual particles
* substituting the delta P in the above equation:
* $$(1-\epsilon_{mf})(\rho_P-\rho)g = 150\frac{(1-\epsilon_{mf})^2\mu v_{mf}}{\epsilon_{mf} ^3 d_p^2}+1.75\frac{(1-\epsilon_{mf})\rho v^2_{mf}}{\epsilon_{mf} ^3d_p}$$
* $$(\rho_P-\rho)g\frac{\rho d_p^3}{\mu^2} = 150\frac{(1-\epsilon_{mf}) v_{mf}d_p \rho}{\epsilon_{mf} ^3 \mu}+1.75\frac{v^2_{mf} d_p^2 \rho^2}{\epsilon_{mf} ^3 \mu^2}$$
* this is after multiplying both sides with:
* $$\frac{\rho d_p^3}{\mu ^2 (1-\epsilon_{mf})}$$
* I dont want to go any further :cry:
