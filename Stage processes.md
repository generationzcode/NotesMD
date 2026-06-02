> Distillation columns contain a number of units connected to each other, called stages. This note explains the terminology and logic behind them. Stage processes can also be applied to leaching and extraction processes

>[!Question]
>	What are the process parameters at every stage? does that matter? Like what is the pressure and temperature at stage n? Why do we not care about it?

>[!Done] Answer
The pressure of the entire column is usually kept constant and the vapor and liquid are kept at equilibrium in steady state - this means they are at their dew and bubble points at each stage. We don't care about this because all of distillation (the chapter) is about material balance, not thermodynamics, not hydrodynamics and maybe we care a little when we get to enthalpy balance instead of assuming [[constant molal overflow]] 

## Terminology
* The stages are numbered using the flow of liquid as the direction. Liquid (usually...) flows downward, so the last stage (of N stages) is the $N^{th}$ stage
* streams flowing out of a unit are subscripted with the number of the stage that it flows out of
* eg. $$L_{n+1},V_{n+1}$$
## Material Balances
* Two types of material balances here - component balance and total material balance
* Total balance: $$V_{n}+L_{n} = V_{n+1}+L_{n-1}$$
* ![[Pasted image 20250120102025.png]]
* Material balance of the whole column: $$L_a+V_b = L_b +V_a$$ where a and b are the components A and B
* component balance: $$L_nx_n+V_ny_n = L_{n-1}x_{n-1}+V_{n+1}y_{n+1}$$
* where x and y are the mole fractions in the liquid and vapour phase of whichever component you're component-balancing
## Enthalpy balance
* $$L_aH_{L,a}+V_bH_{V,b} = L_bH_{L,b}+V_aH_{V,a}$$
* Assuming the process is workless and adiabatic
## Operating line diagram
* A way of showing the compositions of two phases of the stages in an x-y diagram
* The total material balance of a stage is: $$L_a+V_{n+1} = L_n+V_a$$, where L_a is the net liquid coming in, V_a is the net vapour going out, V_{n+1} is the vapour going out of stage n+1 and L_n is the liquid going down into stage n+1
>[!FAQ] To be Understood Later
 V_a-L_a = D for rectification section and L_a-V_a = B for the stripping section
* The component balance of any stage is:
* $$L_ax_a + V_{n+1}y_{n+1} = L_nx_n+V_ay_a$$
* from the component balance, we can get the operating line=>$$y_{n+1} = \frac{L_nx_n}{V_{n+1}}+\frac{V_ay_a-L_ax_a}{V_{n+1}}$$
>[!info] Straight or Curved?
 If the L_n/V_{n+1} remains constant throughout the column, we get a straight operating line, if not, then we gotta make the curvee
