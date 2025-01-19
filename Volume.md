#thermo 
> First years need steam tables and charts. We are now second year

In an explosion, the expansion of a gas is adiabatic

* We need to find out how enthalpy and entropy changes can be calculated as a fucntion of temperature and pressure for real fluids. For this we need how volume changes with temperature and pressure
* Suppose we are compressing CO2 from 50 to 200 bar from 100 degrees C to 200 C.
* ![[Pasted image 20240731101144.png]]
* since we dont know the Cp at 50 or 200 bar, we need to calculate it by taking pressure to 0 at 100 C, temperature to 200 at 0bar, and pressure to 200 bar at 200C to get the enthalpy change:
* $$H_2-H_1 = (H_6-H_1)+(H_7-H_6)+(H_2-H_7)$$
* $$H_2-H_1 = \int_{P_1}^0(V-T\frac{\delta V}{\delta T})_P|_{T_1}dp+\int_{T_1}^{T_2}C_pdT + \int_0^{P_2}[V-T\frac{\delta V}{\delta T}]_P|_{T_2}dP$$
* $$H_2-H_1 = (H_2^{IG}-H_1^{IG})+(H_2^{R}-H_1^R)$$
* $$H^R = \int^P_0[V-T\frac{\delta V}{\delta T}]_P|_TdP$$
* Now looking at entropy:
* $$S_2-S_1 = \frac{C_p}{T}dT-\frac{\delta V}{\delta T}dP$$
* $$S_2^{IG}-S_1^{IG} = \frac{C_p}{T}dT-\frac{R}{P}dP$$
* $$(S_2-S_1) - (S_2^{IG}-S_1^{IG}) = -\int_1^2[\frac{\delta V}{\delta T}_P - \frac{R}{P}]dP = S_2^R-S_1^R$$
* $$S_2-S_1 = (S_2^{IG}-S_1^{IG})+(S_2^R-S_1^R)$$
* Now looking at internal energy:
* $$U_2-U_1 = (U_2^{IG}-U_1^{IG})+(U_2^R-U_1^R)$$
* $$U^R = H^R+PV$$
## V = f(T,P)
* Need an equation valid in any state, liquid or gas and for any fluid
* Lets take water
* The smallest polynomial that will work in fitting P and V is cubic because:
* ![[Pasted image 20240731105552.png]]
* that green line is a cubic equation
* Van der waals relation:
* $$P = \frac{RT}{V-b}-\frac{a}{V^2}$$
* $$aV^3+bV^2+cV+d = 0$$ where a, b c and d are constants and at T_c there is only 1 root for the above equation, is the equation is actually:(a,b are not same here as the equation above)
* $$(V-V_C)^3 = 0$$
* Vc is the critical volume
* $$V^3+(-3V_c)V^2+(3V_c^2)V+(-V_c^3)$$
* so $$a = 1, b=-3V_c, c=3V_c^2, d=-V_c^3$$
* $$Z = \frac{V}{\frac{RT}{P}}$$ is 1 for ideal and not 1 for anything else
* Since Z is a dimensionless number, we like working with it more
* $$(Z-Z_c)^3 = 0$$
* vaan der waal's equation is not very good at predicting Z_c. Inaccurate
## Problem
* Imagine a cylinder of methane at pressure 200 bar and temperature 40C, 0.1m^3
mass of CO2 imagining thatit is ideal gas is 12.3 KG
* Tc, Pc = 190.6K, P_c = 46bar
* a  = 0.23Pa m^6 /gmol
* b = 4.3 * 10^(-5) m^3 /gmol
* Van der waal's equation rearranged for compressibility
* $$Z^3+(-1-B)Z^2+AZ-AB = 0$$
* $$A = \frac{aP}{R^2T^2}, B = \frac{bP}{RT}$$
* $$a = \frac{27R^2T_C^2}{64P_C},b = \frac{RT_C}{8P_C}$$
* A here is 0.6786 and B is 0.3303
* 0.8401 = Z
## Problem
>[!In 11th standard your life was limited to piston and cylinder]
>Imagine we have carbon dioxide at 40C, 15 bar and we want to compress it isothermally to 40C 100 bar. This is done in a piston and cylinder

### Solution
I dont know what the question is I'm just copying the board
$$W = \int^{V_f}_{V_i}\frac{RT}{V-b}-\frac{a}{V^2}dV$$
Tc, Pc = 304K, Pc = 73.76bar
OK thats the solution
## Ok back to serious business
To get vanderwaal's equation explicit in volume for getting H^R and all
$$d(PV) = PdV+VdP$$
$$H^R = \int^{P}_0VdP+\int^P_0T\frac{\delta V}{\delta T}_PdP$$
$$H^R = \int^{PV}_{RT}d(PV) - \int^V_\infty PdV-\int^P_0T(\frac{\delta V}{\delta T}_PdP)$$
The next part I cant understand
$$\frac{\delta V}{\delta T}_P\frac{\delta T}{\delta P}_V\frac{\delta P}{\delta V}_T = -1$$
The above is just a rule for all equations and its just something that is a maths thing not like a thermodynamics thing. So from that, we get:
$$\frac{\delta V}{\delta T}_PdP = -\frac{\delta P}{\delta T}_VdV$$
$$H^R=\int^{PV}_{RT}d(PV)-\int^V_\infty PdV+\int^V_\infty T\frac{\delta P}{\delta T}_VdV$$
$$H^R=PV-RT-\int^V_\infty (\frac{RT}{V-b}-\frac{a}{V^2})dV+\int^V_\infty \frac{TR}{V-b}dV$$
$$H^R/RT = (Z-1)-A/Z$$
$$Sr/R = ln(Z-B)$$

> [!homework]
> FIrst of all you have to find small a and small b, second thing that you have to do is to rearrange in terms of Z^3+Z^2, etc and get A and B. Next thing you have to do is prove this (the differential shit I wrote above). Next thing to do is to integrate the last term of the last equation in that H^R thingy that TDp/dTdv shit. 

