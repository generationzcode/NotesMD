> Make a list of all pipe fittings. Application of all valves. Print/ draw freehand.


>[!problem]
>A reverse osmosis unit for purifying brackish water has 900000 fibres that permit the diffusion of water but reject most of the salt. The fibres are 85 micro meter in outside diameter , 42 micrometers in inside diameter and 3 ft long. The average flow through the tubes is 2000 gallons of water per day when the feed pressure is 400 psig. What is the pressure drop within an individual fibre from the feed end to the discharge end?Assume fluid viscosity = 1cP

## Solution
$$Q = \frac{2000}{264.17*24*60*60} = 8.76*10^{-5}m3/s$$
$$8.76*10^{-5}/(900000*(21*10^{-6})^2*\pi) = 0.07m/s$$
$$Re = 1000*0.07*42*10^{-6}/(10^{-3}) = 2.94$$
$$16/2.94 = f = 5.44$$
$$2*5.44*0.91*1000*0.07^2/(42*10^-6) = \Delta P = 1.155*10^6 Pa$$

>[!Bug]
>Water flows through an 8 inch steel pipe at an average velocity of 6 feet/second. Downstream the pipe divides into an 8 inch main and a 2 inch bypass. The equivalent length of the bypass is 22 feet. Length of the 8 inch pipe in the bypassed section is 16 feet. Neglecting entrance and exit losses, what fraction of total flow passes through the bypass

>[!Solution]
>take point 1 as the end of the bypass and take point 2 as the end of the main
>$$\Delta P_1 = 22*f*2*1000*v^2/d$$
>$$\Delta P_2 = 16*f*2*1000*v^2/d$$
>$$\rho(v_1^2-v_2^2)/2 = \Delta P_2-\Delta P_1$$
>$$v_1= A_2(v_0-v_2)/A_1$$
>$$\rho(\frac{A_2^2*(v_0-v_2)^2}{4A_1^2}-v_2^2)/2 = 6x$$
>Get x2 in terms of x and then get v_1 in terms of x and then multiply that with the respective areas and boom boom bam you get the answer
>$$Re = 1000*1.83*20.32/10^{-3}$$
>$$Re = 371856$$
>$$\Delta P/ L = 2.83*10^{-3}*2*1000*1.8^2/0.2033 = 0.0904$$
>$$0.0904*6 = \rho(\frac{0.00196^2*(1.81-v_2)^2}{4*0.0314^2}-v_2^2)/2 $$
>$$0.0904*6*2/1000+x^2 = (0.00196^2/(4*0.0314^2))*(1.81^2-2*x*1.81+x^2)$$





