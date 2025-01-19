* These guys tried to derive a general equation for pressure drop across packed beds
* They began with getting an analogy between streamline flow in an empty pipe and a packed pipe
* ![[Pasted image 20240925090907.png]]
* ![[Pasted image 20240925091658.png]]
* If free space between particles is assumed to consist of a series of tortuous channels, the hagen poiseuille equation can be rewritten as:
* ![[Pasted image 20240925091938.png]]
* where K1 is a function of the bed structure, and is a dimensionless constant
* Ltube is actually L1 here and is the length of tortuous channel
>[!FAQ]
>What is a tortuous channel?
>randomly formed channels

* The length of a tortuous channel will be higher than the actual length of the pipe.
* V1 and L1 represent conditions in the pores and are not the same as v_avg and packing length. Both will be higher than their normal values
* It is assumed that at any length the length of a tortuous path will be directly proportional to length of a tube
* d1 is the equivalent diameter of the tortuous pore space
* Kozeny said d1 = ![[Pasted image 20240925093749.png]]
* ![[Pasted image 20240925094112.png]]
* K2 accounts for the proportionality between L1 and Ltube and we can use Ltube since we know only Ltube not L1
* 180 = k^2*S
* Modified friction factor is R/pv^2
* ![[Pasted image 20240925100350.png]]
* R1 is drag force, rho is density and v is v1
* for flow to occur, pressure drop is required
* This pressure drop should be exactly equal to the resistance faced by the fluid
* ![[Pasted image 20240925101524.png]]
* $$\frac{R_1}{\rho v_1^2} = \frac{5}{Re_1}+\frac{0.4}{Re_1^{0.1}}$$
* The above is a fitted correlation for packed beds by carman
* It's similar to the equation proposed by Forchheimer, who suggested that resistance to flow should be considered in two parts:
* Viscous force at particle surface
* Loss in turbulent eddies and at sudden changes in cross section of channels, therefore
* $$\Delta P=\alpha v_{avg}+\beta v^n_{avg}$$
* The first term predominates at low flow rates where losses are mainly due to skin friction
* Second term predominates at high flow rates and in very thin beds where the enlargement and contraction losses become very important. AT very high flow rates the effects of viscous forces are negligible
* For Re < 2, second term = 0, hence
* $$\frac{R_1}{\rho v_1^2}=\frac{5}{Re_1}$$
* Learn the derivation of the Forchheimer equation
* Sawitowski proposed for flow of fluids through hollow packings:
* $$\frac{R_1}{\rho v_1^2} = \frac{5}{Re_1}+\frac{1}{Re_1^{0.1}}$$
* Note the lack of 0.4 on the numerator of the second term
* For flow through ring packings, another relation was created (semi empirical):
* $$\frac{\Delta P}{L_{tube}} = 150\frac{(1-\epsilon)^2\mu v_{avg}}{\epsilon ^3 d_p^2}+1.75\frac{(1-\epsilon)\rho v^2_{avg}}{\epsilon ^3d_p}$$
* This is analogous to hejun poisuelle equation
* Using 6/S, it transforms to something else
* This is not worth remembering and thus I wont write about it here
* All these equations will be provided in the exam
> [!Important]
> Prof's recommendation - When designing a packed bed column there are softwares that fit a curve on the packed column readings and get you a relation
