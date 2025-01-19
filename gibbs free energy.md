#thermo 
BAD TITLE, it has a lot more than GFE
$$\frac{d}{dt}(U^t+PV-TS) = \sum{m_i(H_i-TS_i)}+\dot{w_s}$$
This gives maximum possible work that can be extracted from a process
$$\frac {dU^t}{dt}+P_e\frac{dV}{dt}+T\frac{dS^t}{dt} = \sum{mH_i} - \sum{mTS_i} + \dot{w_s}-TS^t_{gen}$$
Gibbs energy requires isothermal conditions

$$B=H-T_oS$$ T_o is the ambient temperature, matter of notation use 300K
>[!note]
>$$S^t_{gen}>=0$$


$$G=U+PV-TS$$
or
$$G=H-TS$$

or
$$\frac{dG^t}{dt} = \sum{m_iG_i} +W_s-TS^t_{gen}$$
>B,X and G are just different ways of looking at systems, you can use anything even U and S to evaluate stuff

$$dU = TdS-PdV$$
$$dH = TdS+VdP$$
$$dG=VdP-SdT$$
thus
$$dH = \frac{\delta H}{\delta T}_PdT + \frac{\delta H}{\delta P}_TdP$$
=> $$(\frac{\delta H}{\delta P})_T = T(\frac{\delta S}{\delta P})_T+V$$
=> $$\frac{\delta G}{\delta P}_T = V$$
=>$$\frac{\delta}{\delta T}.(\frac{\delta G}{\delta P})_T = (\frac{\delta V}{\delta T})_P$$
=> $$\frac{\delta G}{\delta T}_P = -S$$
=>$$\frac{\delta}{\delta P}.(\frac{\delta G}{\delta T})_P = -(\frac{\delta S}{\delta T})_T$$
=> $$\frac{\delta V}{\delta T}_P = -\frac{\delta S}{\delta T}_T$$
=> $$dH = C_pdT+[V+T(\frac{\delta S}{\delta T})_T]dP$$
=> $$dH = C_pdT+[V-T(\frac{\delta V}{\delta T})_P]dP$$
=> $$dS = \frac{\delta S}{\delta T}_P+{\frac{\delta S}{\delta P}}_TdP$$
=> $$dS = \frac{C_p}{T}dT-\frac{\delta V}{\delta T}_TdP$$
## Ideal Gas
PV = RT
$$\frac{\delta V}{\delta T}_P = \frac{R}{P}$$
$$dH = C_PdT +[V-\frac{\delta V}{\delta T}T]dP$$
$$dH = C_pdT$$
___
$$dS = \frac{C_p}{T}dT-\frac{R}{P}dP$$
integrating,$$S_2-S_1 = C_pln\frac{T_2}{T_1} - R ln\frac{P_2}{P_1}$$
$$C_pln\frac{T_2}{T_1} = R\ ln\frac{P_2}{P_1}$$
## Liquids
$$dH = C_pdT+[V-T\alpha V]dP$$
Alpha is the coefficient of thermal expansion (volumetric)
> [!problem]
> water from 30 to 50 degrees celsius, 1 to 100 bar
> to get enthalpy change, we take the above equation at constant pressure to 50 degrees celsius then at constant temp from 1 to 100 bar

$$dS = \frac{C_p}{T}dT+\frac{\delta V}{\delta T}dP$$
>[!problem]
>We have a process, a secret process in which air comes in at 2kg/s, 20C, 4bar. 1kg/s comes out at 60C, 1 bar, 1 kg comes out at -20C, 1 bar. Is this process possible?

### Solution
Let S for stream 1 be 0
$$S = \int^{60+273}_{20+273}\frac{0.24*4.2}{T}dT+\int^1_4\frac{8.31*1000/28.4}{P}dP$$
$$S = 0.129+0.4$$
$$S=-0.148+0.4$$
$$S_{gen} = 0.61$$
ITS FEASIBLE
LOL
>[!problem]
>Do exergy balance. Heat exchanger with 4 streams. One of liquid **stuff** with $C_p = 0.5kcal/KgK$ coming in at $10,000Kg/Hr$.inlet and outlet are 150 and 60C. The other of cooling water between 40 and 30C

### Solution
How much cooling water needed?
$$\frac{(0.5*10000*90)}{1*10} = m_w = 45000Kg/Hr$$
the exergy difference between liquid stuff:
$$\Delta X = \Delta H - T_\sigma \Delta S$$
$$\Delta S = \int^{273+60}_{273+150}\frac{C_p}{T}dT = -0.5 = -5023$$
$$\Delta X = -0.5*4.2*90*10000+300*5023 = -383,100KJ$$
The exergy balance for the water
$$\Delta X = \Delta H-T_\sigma\Delta S$$
$$\Delta S = \int^{40+273}_{30+273}\frac{C_p}{T}dT = 0.136 = 6136$$
$$\Delta X = 1*4.2*10*45000-300*6136 = 49200$$
exergy total balance 
$-333900KJ/Hr$
$S_{gen} = 1113KJ/HrK$
> Note - I did out-in not in-out so the signs are a bit odd. Rest assured thermodynamics hasnt failed us

>NOTE NUMBER 2 - SINCE ENTHALPY BALANCE EXISTS, THE H PART OF X CANCELS OUT CUS NET H IS 0, SO IT ENDS UP BEING T_NAUGHT (DELTA S) EPIK EPIK EPIK
==AHYOAHEYOAHEYAOEH IM RIGHT LOL==
---

## Compreshun
imagine we are compressing air from 30C, 1 bar to 10 bar pressure unknown temp
$$dS = \frac{C_p}{T}dT -\frac{R}{P}dP$$
$$\frac{a+bt+ct^2+dt^3 +. . .}{T}dT+\frac{R}{P}dP = dS$$
we need multistage compressors because no material on earth can handle a temperature difference of more than probably 100 or 200 (not metal and can be used on the oaring of a compressor to have 0 tolerance)

in multistage compressors we need compression ratios that are equal between all the compressors so the work done is minimized (this is left as an exercise for myself) - easy shit
>[!problem]
>we got a pump, we got a box, we try to take out air from box isothermally until vacuum from 1 bar. Compressor is adiabatic

### Solution
$$H_2-H_1$$
What is enthalpy of the system at start?
its H=U+PV
=> $nC_v*T+10^5*1$
=> 712 * 300 * 1.157+10^5
