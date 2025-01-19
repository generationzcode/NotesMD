* Two types of resistances with cake resistance - cake and filter medium
* Filter medium resistance - considered when starting up
* Cake resistance - zero at startup and increases with time
* let pa = inlet pressure
* pb = outlet pressure
* p' pressure at boundary between cake and filter medium
* Then,
* $$\Delta P = pa-pb = (pa-p')-(p'-pb) = \Delta P_C+\Delta P_M$$
* where del Pc is cake pressure drop and Pm is the filter medium pressure drop
* Consider a thin layer of cake having differential thickness dL, situated at a distance of L from the filter medium
* Let p = pressure at above point
* Assume: the velocity in the filter bed is low enough for it to be in laminar flow
* We use the [[Carman Kozeny equations]] for laminar flow in a packed bed
* $$\Delta P/L = \frac{150*\mu*u(1-\epsilon)^2}{g_c(\Phi_SD_p)^2\epsilon^3}$$
* we are more fond of specific surface here so we substitute:
* $$\frac{6V_p}{S_p} = \Phi_pD_p$$
* $$\Delta P/L = \frac{4.17*\mu*u(1-\epsilon)^2}{g_c(V_p/S_p)^2\epsilon^3}
$$
## Applying carman kozeny to filtration
* The linear velocity at time,t:$$v = u = \frac{dV}{dt}/A$$
* Volume of solids in the differential layer = $$AdL(1-\epsilon)$$
* Mass of solids in the differential layer = $$dm = \rho_pAdL(1-\epsilon)$$
* substituting dL in carman kozeny equation:
* $$dP = \frac{K_1\mu u (1-\epsilon)(S_p/V_p)^2}{\epsilon^3\rho_pA}dm$$
* the filtration equation $$\Delta P =  \frac{K_1\mu u (1-\epsilon)(S_p/V_p)^2}{\epsilon^3\rho_pA}m$$
* Specific cake resistance: $$\alpha = \frac{\Delta P_cA}{\mu u m_c} = \frac{k_1(1-\epsilon)(S_p/V_p)^2}{\epsilon^3\rho_p}$$
* Cake resistance: $$\alpha m_c/A = \Delta P_c/(\mu u)$$
* For incompressible cakes, alpha is not a function of delta P
* filter medium resistance: $$R_m = \frac{P'-P_b}{\mu u} \approx 10^{10}-10^{11}$$
* $$\Delta P = \mu u(m_c\alpha/A+R_m)$$
* At an appreciable cake thickness, \delta p_m is negligible and only cake resistance counts towards the total pressure drop
* If C = m_c/V, then total cake mass is mc = C* V
* also u = (dV/dt)/A
* Thus: $$\Delta P = \mu \frac{dV}{Adt}(CV\alpha/A+R_m)$$