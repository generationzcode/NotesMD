## Double Pipe
- This is easy, there is are two pipes, one inside the other. The annulus is filled with thermal fluid, so is the cylinder inside. The annulus and inner pipe exchange heat with each other through the wall of the inner pipe. In this case, we actually have about 5 films. but usually the outer pipe is well insulated so we can just assume 3 films - the fluid in the inner pipe, the fluid in the outer pipe and the wall between them.
- The heat transfer coefficients are calculated using the sieder tate equation to get the Nusselt number. the The heat transfer coefficient of the wall is taken to be disproportionately large
- These double pipes can be sized (the size of the heat exchanger if the heat duty and temperatures are given) using LMTD approach, less so by $\epsilon$-NTU method
- The $\epsilon$-NTU method is used to mostly rate heat exchangers since the LMTD method needs some amount of trial and error to work here
## Shell and Tube
- ![[Pasted image 20250325160207.png]]
- Its easy to get the heat transfer coefficient of the fluid in the inner tubes, but to get the heat transfer coefficient of the fluid in the shell side, we need the donohue correlation for the nusselt number
- ![[Pasted image 20250325160322.png]]where G_e is square root of the mass velocity of the fluid in the shell side flowing parallel to the tubes and the mass velocity of the fluid on the shell side flowing in cross current to the tubes. 
- This is because the fluid in a shell and tube heat exchanger faces baffles and thus flows both cross current as well as parallel
## Plate type
- McCabe and Smith have un-refreshingly little information on these
- Usually operated at low pressures of below 20atm, plates separated by 5mm and run viscous fluids
- The nusselt number is related by $$Nu = CN_{Re}^{0.4}N_{Pr}^{0.3\space or\space 0.64\space for \space turbulent}$$
- 