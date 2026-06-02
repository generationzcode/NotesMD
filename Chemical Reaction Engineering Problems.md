![[Pasted image 20250121112357.png]]
>[!Danger] Question
>A-> B is carried out in a CSTR, $F_{AO} = 0.4gmol/s$, calculate the volume necessary to get 80% conversion in CSTR, or spacetime for 80% conversion
>

>[!Done] Solution
>
| $x_A$ | -$r_A$ $gmol m^{-3}s^{-1}$ | $-\frac{1}{r_A}$ $m^3sgmol^{-1}$ |
| ----- | -------------------------- | -------------------------------- |
| 0     | 0.45                       | 2.22                             |
| 0.1   | 0.37                       | 2.70                             |
| 0.2   | 0.30                       | 3.33                             |
| 0.4   | 0.195                      | 5.13                             |
| 0.6   | 0.113                      | 8.85                             |
| 0.7   | 0.079                      | 12.7                             |
| 0.8   | 0.05                       | 20                               |
![[Pasted image 20250114085807.png]]


>[!Danger] Data Problem
>A reaction A->R gives the data on starting reaction from C_a0 = 1gmol/litre
>![[Pasted image 20250116085351.png]]
>the left column is the conc in gmol/m3 and right is time(actually the other way round sorry)
>how much will the conversion at 300min be if the reaction starts at half c_a0? -> 
>

>[!done] Solution 
>60%


>[!Danger] Levenspiel 3.24

>[!Done]
	
	import matplotlib.pyplot as plt
	CA = [1,2,4,6,7,9,12]
	ra = [0.06,0.1,0.25,1.0,2.0,1.0,0.5]
	def interpolate_kewl(op):
	    for v,i in enumerate(CA):
	        if i>=op:
	            p1 = [CA[v-1],ra[v-1]]
	            p2 = [CA[v],ra[v]]
	            break
	    slope = (p2[1]-p1[1])/(p2[0]-p1[0])
	    return slope*(op-p1[0])+p1[1]
	arr_eval = np.linspace(1,12,100)
	time_spend = 0
	time = []
	for i in arr_eval:
	    time_spend+=(11/100)/interpolate_kewl(i)
	    time.append(time_spend)
	plt.plot(arr_eval,time)
	plt.show()

![[Pasted image 20250121100913.png]]
