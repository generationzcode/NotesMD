### Shear stress and skin friction in pipes
![[Pasted image 20240723105856.png]]
The black thing in the center is a cylinder of radius r and the tube is of radius R, it has length dl. Pressure at the left side is P, pressure at the right side is P+dP
The tube has a liquid travelling in laminar flow
* the shear stress is $\tau$ at the surfaces of the black cylinder
* $$-\pi r^2dp = \tau*2\pi r*dl$$
* $$-\frac{dP}{dz} = \frac{2\tau}{r}$$
* at r = R (pipe wall)
* $$\frac{dP}{dz} = -\frac{2\tau_w}{R}$$
* the above is the pressure gradient in a laminar flow pipe for a specific shear stress
* equation$$P_2-P_1 = -\frac{4\tau_wL}{D}$$
* fanning friction factor:
* $$f=\frac{2\tau_w}{\rho v_{av}^2}$$
* eliminating $\tau_w$ in these two equations$$\frac{\Delta P_{fric}*D}{2L\rho v_{av}^2}=f$$
  $$\Delta P = \frac{2fL\rho v_{av}^2}{D}$$
  equation of motion, cylindrical coordinates gives a velocity profile in a circular pipe, smooth, constant cross section, laminar flow:
  $$v_z = \frac{\Delta P_{fric}D^2}{16\mu L}[1-(\frac{r}{R})^2]$$
  Parabolic profile
  ![[Pasted image 20240723115032.png]] 
  something like this
  This is in **no slip condition**
  * No slip condition states that in case of fluid solid contact,velocity of fluid is equal to velocity of solid
  * to get the flow rate:
  * take the differential area like this :
  * ![[Pasted image 20240723120502.png]]
  * $$Q = \int^R_0v_z*2\pi rdr$$
  * $$v_{av} = \frac{Q}{\pi R^2}$$
  * $$v_{av} = v_{max}/2$$
  * THIS ABOVE RELATION IS JUST A COINCIDENCE AND NOT BECAUSE $(V_{MAX}-0)/2$ IS AVERAGE
  => $$\frac{D^2(\Delta P_{fric})}{32\mu L} = v_{av}$$
  =>$$\Delta P_{fric} = \frac{2fL\rho v_{av}^2}{D}$$
  => $$f = \frac{16\mu}{D\rho v_{av}}$$
  =>$$f=\frac{16}{Re}$$
  A smooth pipe is one with no obstruction inside it - NOT FRICTIONLESS you egg
  $$Re = \frac{Dv_{av}\rho}{\mu}$$
  