* To measure flow rate, we need $\Delta P$, and this must be measurable
>[!HIstorically Accurate Story] 
>Two italians eating pizza on sicily islands and they generally discuss flow measurement. They realized that without flow measurement, life is nothing. The italians then solved the problem of flow measurement. The two italians were Venturi and Bernoulli
* The points between pressure measurement are so small that frictional losses are negligible
* The venturi coefficient is a measurement of frictional losses
* $$\frac{P_1}{\rho g}+\frac{v_1^2}{2g}+h_1=\frac{P_2}{\rho g}+\frac{v_2^2}{2g}+h_2$$=>(1)$$\frac{P_1}{\rho g}+\frac{v_1^2}{2g}=\frac{P_2}{\rho g}+\frac{v_2^2}{2g}$$
 ![[Pasted image 20240718105744.png]]
* Outlet angle is less than inlet so that the divergent flow doesn't cause vortices
* The narrow middle part is the throat
* There are 3 tappings, one at the converging area, one at the throat and one at the divergent section. The divergent area is the pressure recovery section
* Using (1) here, we can get the velocity difference at the two points
* Point 1 is sufficiently upstream, while point 2 is at the midpoint of the throat or end of the throat
* Use equation of continuity:
* $$v_1 =\frac{A_2v_2}{A_1}$$
=>$$\frac{P_1-P_2}{\rho g} = \frac{-(\frac{A_2v_2}{A_1})^2+v_2^2}{2g}$$
=> $$2\frac{P_1-P_2}{\rho} = (1-(\frac{A_2}{A_1})^2)v_2^2$$
=>$$v_2 = \sqrt{\frac{2(P_1-P_2)}{-\rho(\frac{A_2}{A_1})^2+\rho}}$$
=>$$V = A_2\sqrt{\frac{2(P_1-P_2)}{\rho-\rho(\frac{A_2}{A_1})^2}}$$

$$\frac{d_2}{d_1} = \beta$$ in all the textbooks, where d is the diameter
Prof's formula = 
$$v_2 = \sqrt{\frac{2\Delta P}{\rho(1-\beta^4)}}$$
### Discharge coefficient
* $C_o$ just multiply this with the above formula
## [[Problem on venturi meter]]