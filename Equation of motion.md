#fluidmech 
> [!Warning]
> This will be tricky
## Three big conditions
* On a solid fluid boundary, fluid layers adjacent to the solid move with the same velocity as the solid - This is the no slip condition
* For liquid gas interface, the shear stress is negligible. 
* For liquid liquid interface, the shear stress is continuous over the interface. The momentum flux is perpendicular to the interface
## Introduction
* Equation of continuity is mass rate balance and equation of motion is a momentum rate balance
> Try and understand the equation of motion
* The diagram, while I cannot draw right now, is very similar to the equation of continuity
* the things moving through are the momenum fluxes
* There are two types of stresses, conductive (viscous) stress and convective stress
* Equation of motion is developed by writing a momentum balance over a volume element fixed in space, through which a fluid is flowing
* $${ momentum\space accumulation\space rate } = momentum \space in \space rate-momentum \space out \space rate+external\space force \space on \space fluid$$
* x component is developed as follows, convective and molecular transport (conductive)
* Rate at which x momentum enters and leaves the faces at x and x+$\Delta X$ are (convective)$$(\Phi_{xx})_x\Delta Y \Delta Z\space and \space (\Phi_xx)_{x+\Delta x}\Delta Y \Delta Z$$
* Rate at which x momentum enters and leaves the faces at Y and Y+$\Delta Y$ are (Conductive)$$(\Phi_{YX})_Y\Delta Z \Delta X\space and \space (\Phi_YX)_{Y+\Delta Y}\Delta X \Delta Z$$
* Rate at which x momentum enters and leaves the faces at Z and Z+$\Delta Z$ are (Conductive)$$(\Phi_{ZX})_Z\Delta Y \Delta X\space and \space (\Phi_ZX)_{Z+\Delta Z}\Delta X \Delta Y$$
* Addition of the above 3 components gives the net rate of addition of x momentum. 
## In the Y and Z directions
### Y
* Rate at which Y momentum enters and leaves the faces at x and x+$\Delta X$ are (convective)$$(\Phi_{YX})_x\Delta Y \Delta Z\space and \space (\Phi_{YX})_{x+\Delta x}\Delta Y \Delta Z$$
* Rate at which Y momentum enters and leaves the faces at Y and Y+$\Delta Y$ are (Conductive)$$(\Phi_{YY})_Y\Delta Z \Delta X\space and \space (\Phi_{YY})_{Y+\Delta Y}\Delta X \Delta Z$$
* Rate at which Y momentum enters and leaves the faces at Z and Z+$\Delta Z$ are (Conductive)$$(\Phi_{ZY})_Z\Delta Y \Delta X\space and \space (\Phi_{ZY})_{Z+\Delta Z}\Delta X \Delta Y$$
### Z
you know how to do this

## Finishing in X
* Net rate of addition of X-momentum is:
* $$\Delta Y\Delta Z ((\Phi_{xx})_x-(\Phi_{xx})_{x+\Delta x})+\Delta X\Delta Z ((\Phi_{yx})_y-(\Phi_{yx})_{y+\Delta y})+\Delta X\Delta Y ((\Phi_{zx})_z-(\Phi_{zx})_{z+\Delta z})$$
* In addition there is an external force (typically the gravitation) acting on the fluid in volume element. X component of this force is (mass * g_x basically lol). The g_x is the g in the x direction, which is 0 na lmao $$\rho g_x \Delta X\Delta Y\Delta Z$$
* Total of the above 4 terms gives x-component only, and should be equal to the rate of accumulation of x-momentum within the volume element
* $$\Delta X\Delta Y\Delta Z [\frac{\delta(\rho v_x)}{\delta t}]$$
* This gives: $$\Delta Y\Delta Z ((\Phi_{xx})_x-(\Phi_{xx})_{x+\Delta x})+\Delta X\Delta Z ((\Phi_{yx})_y-(\Phi_{yx})_{y+\Delta y})+\Delta X\Delta Y ((\Phi_{zx})_z-(\Phi_{zx})_{z+\Delta z})+\rho g_x \Delta X\Delta Y\Delta Z=\Delta X\Delta Y\Delta Z [\frac{\delta(\rho v_x)}{\delta t}]$$
* dividing both sides by the control volume:
* $$\frac{\delta (\rho v_x)}{\delta t} = -(\frac{\delta (\Phi_{yx})}{\delta y}+\frac{\delta (\Phi_{xx})}{\delta x}+\frac{\delta (\Phi_{zx})}{\delta z})+\rho g_x$$
* similarly can be written for y and z elements
* phi actually contains both convective and molecular transport elements
* $$\frac{\delta (\rho v_x)}{\delta t} = -(\frac{\delta (\tau_{yx})}{\delta y}+\frac{\delta (\tau_{xx})}{\delta x}+\frac{\delta (\tau_{zx})}{\delta z})-(\frac{\delta (\rho v_x v_y)}{\delta y}+\frac{\delta (\rho v_x v_x)}{\delta x}+\frac{\delta (\rho v_x v_z)}{\delta z})-\frac{\delta P}{\delta x}+\rho g_x$$
* > Equation of motion should actually be called equation of momentum/force. It has convective forces, conductive forces and external forces (pressure and gravity)
## Tau
* It's stress. Very difficult to explain without a diagram, but I forgot the graphics tablet in my room. 
* IN 2D:
* Tau yx is the viscosity multiplied by the gradient of x velocity with respect to y
* Tau zx is the viscosity multiplied by the gradient of x velocity with respect to z
* Tau xx is the viscosity multiplied by the gradient of x velocity with respect to x
* Tau xx, Tau yy, Tau zz are all direct stresses due to viscosity
* IN 3D:
* $$\tau_{yx} = -\mu (\frac{\delta v_x}{\delta y}+\frac{\delta v_y}{\delta x})$$
* what a nightmare to visualize... 
* analogously (?) you can get this for all the other components - yz,xz
* $$\tau_{xx} = -2\mu \frac{\delta v_x}{\delta x}$$
* analogously (?) you can get the tau for all other components - yy,xx
* expand the convective stresses if you want using the product rule
> Home assignment number 8 and 9, r and theta derivation of equation of motion in cylindrical coordinates

## Fluid mechanics paper question 1
* vr = 0 thus all components with v_r are zero
* Since no gravity is in radial direction - so rho g_r is also 0
* same with theta