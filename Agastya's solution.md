>[!IMportant]
>Agastya appreciation note for actually trying to solve this problem, when I disregarded it


If I had more time, I'd run a gradient descent or genetic algorithm on the guess parameters to better find the global minimum. I enjoy sleep so I avoided that - heres the solution. Pretty simple but feels weird to make a CSTR a constraint :/

>[!info]
>The gauss seidel solver is an early implementation, primarily because I didn't know it was gauss seidel. The idea was just some *jugaad* method of getting rate of R to get the space time to get the volume of the reactor given the constraints. It was pointed out to me by a professor that I was simply solving a system of linear equations later on. Apologies to the applied math 2 professor for not remembering gauss seidel. The engineer in me just likes *jugaad*
>
>For similar problems, I suggest using a standard algorithm for gauss seidel and proper definition of the equations involved.
>
>Also the last part regarding the guess params can be improved, for any ML engineers here, please help find the global minimum in the most sophisticated manner




![[Pasted image 20240809214724.png]]
```
# Modify this for any backmix system or mixed flow model with any number of reactions occurring
def func2(guess_params):
  def func(x):
    a,b = x[0],x[1]
    # Making sure the parameters being minimized don't break physics
    if any(value < 0 for value in x):
      return float('inf')
    if (0.1*a-100)<0 or (0.1*b-100)<0:
      return float('inf')
    # Gauss seidel guess values
    RateR = 100/(a+b)
    rateS=0.01
    space_time = 1
    # Gauss seidel iteration below
    for i in range(1000):
      rateS = 34.4*((0.1*b-100-2*rateS*(a+b)*space_time)**2)/((a+b)**2)
      rateR = (68.8*(0.1*a-100)*(0.1*b-100-2*rateS*(a+b)*space_time))/((a+b)**2)
      space_time = 100/((a+b)*rateR)
    Volume = space_time*(a+b)
    # Just to be sure we aren't minimizing below 0 for cost
    if  (0.5*a*0.1+0.5*b*0.1+Volume*0.01) <0 or rateR<0 or rateS<0:
      return float('inf')
    return (0.5*a*0.1+0.5*b*0.1+Volume*0.01)
  # Initial guess for the parametersds
  x0 = guess_params
  from scipy.optimize import minimize
  # Minimize the function
  result = minimize(func, x0, method='Nelder-Mead')

  # Print the minimized values
  print("Minimized values:", result.x)
  print(func(result.x))
  return result.x


# The below is just to be sure that the gradient descent doesnt end up finding a local minimum
from random import randint
pms = [1700,1100]
for i in range(20):
  pms = func2([pms[0]+(randint(0,100)-50),pms[1]+(randint(0,100)-50)])

```

```
Minimized values: [1745.65901605 1074.98147565]
141.03203154468133
Minimized values: [1749.25484058 1096.36791454]
142.28434645926865
Minimized values: [1727.19721205 1123.38967466]
142.5297585458841
Minimized values: [1785.86732074 1074.83077385]
143.06724796114523
Minimized values: [1779.62761719 1160.05076387]
146.99008063965456
Minimized values: [1750.35795958 1198.40546874]
147.43821223967868
Minimized values: [1687.00587764 1152.99203794]
142.01527974715393
Minimized values: [1768.44290658 1088.42321157]
142.84330739763575
Minimized values: [1629.02049763 1075.55274758]
135.30726884488664
Minimized values: [1644.02584969 1087.98636355]
136.6006238427965
Minimized values: [1704.78088112 1108.04585912]
140.6479785601245
Minimized values: [1630.26409807 1147.54872532]
138.89064657092823
Minimized values: [1611.79175508 1153.69072188]
138.34366513117212
Minimized values: [1483.62357463 1329.69960106]
144.73993286193405
Minimized values: [1433.55258628 1356.80995142]
142.09858792197588
Minimized values: [1432.05071922 1351.90345207]
141.68282483571912
Minimized values: [1439.90847981 1347.5703457 ]
142.47549657556476
Minimized values: [1617.73928642 1279.83544326]
144.8834690342785
Minimized values: [1540.21634085 1319.35975845]
204.40996698200632
Minimized values: [1684.86278723 1302.28615475]
149.35820255652848
```
