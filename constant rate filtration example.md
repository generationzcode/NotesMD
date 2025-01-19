# Constant rate

```python
import matplotlib.pyplot as plt
import numpy as np
import scipy
delP = [0.4,0.5,0.7,0.8,1.1,1.2,1.3]
delP = np.array(delP)*10**5
t = [447,851,1262,1516,2167,2552,2909]
a=1
b=100
def f(a,b,x):
    return a*x+b
def error(arr,x_arr,y_arr):
    a=arr[0]
    b=arr[1]
    return np.mean((y_arr-f(a,b,x_arr))**2)
p_pred = f(scipy.optimize.minimize(error,np.array([a,b]),args=(np.array(t),np.array(delP))).x[0],scipy.optimize.minimize(error,np.array([a,b]),args=(np.array(t),np.array(delP))).x[1],np.array(t))
plt.scatter(t,delP)
plt.plot(t,p_pred)
plt.show()
a,b= scipy.optimize.minimize(error,np.array([a,b]),args=(np.array(t),np.array(delP))).x
V = np.array([0.04,0.07,0.1,0.13,0.17,0.19,0.22])
q = np.mean(V[1:]-V[:-1])/(t[-1]-t[0])
A = 0.6**2
C = 0.1
mu = 0.001
alpha = (A**2)*a/(C*mu*q**2)
Rm = (A*b)/(mu*q)
```

![png](output_4_0.png)

```python
alpha
```
    np.float64(336645104361088.94)
```python
Rm
```
    np.float64(627148332376.8004)

