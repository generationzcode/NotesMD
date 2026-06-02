## Non Interacting
- Two tanks, one outflow into the other
- Let us consider F_i as flow in, F_1 as the outflow from the first tank and inflow into the second and F_2 as the outflow from the second tank
>[!Info]
>Here we can see that the level in the second unit has no effect on the first unit, but the level in the first unit affects the second unit. This is called non interacting

- $$F_1 = k_1\sqrt{H_1}$$
- $$F_2 = k_2\sqrt{H_2}$$
- So what will happen to the height in the second tank when the flow in the first tank is changed
- Mass balance:$$A_0\frac{dh_1}{dt} = F_i-k_1\sqrt{h_1}$$ for tank 1 and $$A_1\frac{dh_2}{dt} = k_1\sqrt{h_1}-k_2\sqrt{h_2}$$
- converting to deviation variables(non steady state from steady state): first tank - $$A_0\frac{d(h_1-h_{1s})}{dt} = A_0\frac{d\bar h}{dt} = \bar F_1 - \bar h_1\frac{k_1}{2\sqrt{h_{1s}}}=\bar F_1-\frac{\bar h_1}{R_1}$$
- => $$A_0 s \bar h_1(s) = \bar F_1(s)-\frac{h_1(s)}{R_1}$$
-  $$(A_1R_1)s\bar h_1(s) = R_1\bar F_1(s)-\bar h_1(s)$$
- => $$[(A_1R_1)s+1]\bar h_1(s) = R_1\bar F_1(s)$$
- =>$$\tau\bar h_1(s) = R_1\bar F_1(s)$$
- The gain function: $$\frac{\bar h_1(s)}{\bar F_i(s)} = \bar R_1/\tau$$
- For the second tank: $$\frac{A_2d\bar h_2(t)}{dt} = \frac{k_1}{2\sqrt{h_1s}}\bar h_1-\frac{k_2}{2\sqrt{h_2s}}\bar h_2$$
- =>$$A_2sh_2(s) = \bar h_1/R_1+\bar h_2 /R_2$$
- =>$$(A_2s+\frac{1}{R_2})\bar h_2(s) = \frac{\bar h_1(s)}{R_1}$$
- =>$$(\tau s+1)\bar h_2(s) = \frac{R_2}{R_1}\bar h_1(s)$$
- so gain function:
- $$\frac{\bar h_2(s)}{\bar h_1(s)} = \frac{R_2/R_1}{\tau s+1} = G$$
- so the **ULTIMATE Gain Function**$^{TM}$ is the two gains multiplied with each other:$$G_{ULTIMATE^{TM}} = \frac{R_2}{\tau(\tau s+1)}$$
## Interacting
- Now we have two tanks connected to each other on the same level and one has inlet flow and they're connected to each other
- Steady state input flow rate is 10m^3/hr ,h_1 = 2m, h_2=1.5m, A1,A2 = 1m^2, Unsteady state is when there is a 10% increase in flow rate
- so the mass balance: $$A_1\frac{dh_1}{dt} = F_i-k_1\sqrt{h_1-h_2}$$ and $$A_2\frac{dh_2}{dt} = k_1\sqrt{h_1-h_2}-k_2\sqrt{h_2}$$
- Ok so if anyone wants to know how to solve this - you first linearize the DE to make it a linear DE so all the h1, h2 must be to the power 1, the second equation will need a multivariable taylor series
- the second thing you do is create the equations for steady state and minus them from these to get everything in deviation variables. Of course, you could do it without that little prop also, but the book says we have to do it this way, so there must be some edge case out there.
- Finally you laplace transform it all, separate it and back,and you've solved it