#thermo 
Using python for the PR EOS:
```
import numpy as np
import numpy
import math
import matplotlib.pyplot as plt
def get_derivative(x,TC,PC,P):
  return ((piss(TC,PC,x+0.001,P)[0]-piss(TC,PC,x-0.001,P)[0])/(2*0.001))
def piss(TC,PC,T,P):
  w = 0.344
  T_r = T/(TC)
  R = 8.314
  k = 0.37464+1.54226*w-0.26992*w**2
  alpha = (1+k*(1-math.sqrt(T_r)))**2
  a = (0.45724*alpha*R**2*TC**2)/PC
  b = 0.0778*(R*TC)/PC
  return (a,b)
def roots_nikaal(TC,PC,T,P):
  R = 8.314
  a,b = piss(TC,PC,T,P)
  A = a*P/((R**2)*(T**2))
  B = b*P/(R*T)
  roots_lol =np.roots([1,B-1,A-3*B**2-2*B,B**2+B**3-A*B])
  rootz= [np.max(roots_lol),np.min(roots_lol)]
  HRL = 8.31*T*(rootz[0]-1+((T*get_derivative(T,TC,PC,P)-a)/(2*math.sqrt(2)*b*(R*T))*numpy.log((rootz[0]+(1+math.sqrt(2))*B)/((rootz[0]+(1-math.sqrt(2))*B)))))
  SRL = 8.31*(numpy.log(rootz[0]-B)+((get_derivative(T,TC,PC,P))/(2*math.sqrt(2)*b*R))*numpy.log((rootz[0]+(1+1.41)*B)/(rootz[0]+(1-1.41)*B)))
  HRG = 8.31*T*(rootz[1]-1+((T*get_derivative(T,TC,PC,P)-a)/(2*math.sqrt(2)*b*(R*T)))*numpy.log((rootz[1]+(1+math.sqrt(2))*B)/((rootz[1]+(1-math.sqrt(2))*B))))
  SRG = 8.31*(numpy.log(rootz[1]-B)+((get_derivative(T,TC,PC,P))/(2*math.sqrt(2)*b*R))*numpy.log((rootz[1]+(1+1.41)*B)/(rootz[1]+(1-1.41)*B)))
  GRL = HRL-T*SRL
  GRG = HRG-T*SRG
  return [np.exp(GRL/(R*T)),np.exp(GRG/(R*T))]
G1 = []
G2 = []
P = []

for i in range(1000,6000):
  G1.append(roots_nikaal(643,220*10**5,273+200,i*1000)[0])
  G2.append(roots_nikaal(643,220*10**5,273+200,i*1000)[1])
  P.append((i*1000)/(10**5))
plt.plot(P,G1)
plt.plot(P,G2)
plt.xlabel("Pressure(Bar)")
plt.ylabel("fugacity(Pa/mole)")
plt.show()
```
Ignore the inappropriate naming system we implemented in frustration
![[Pasted image 20240814163039.png]]
so the vapour pressure is around 17 bar. This is close enough