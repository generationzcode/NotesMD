Lets take a predator and prey situation
- The predator numbers can be expressed as:
- $$\frac{dP}{dt} = caNP-dP$$
- The prey can be represented as:
- $$\frac{dN}{dt} = rN(1-\frac{N}{K})-aNP$$
- From this, we want dN/dt = dP/dt = 0 situation. We can clearly see some boundary and trivial conditions: (N,P) = (0,0) , (K,0). The equilibrium point where there is no extinction of either species is (N*,P*)
- This can be evaluated by solving the linear equations
- We can further extend this idea to more complicated equations that can't be solved so easily:
## Stability Analysis
- You use a jacobian matrix for this
- Find the derivatives with respect to N and P for the predator in the first row and in the second row, find the derivatives with respect to N and P for the prey
- Once you're done with this, find the eigenvalues
- If even one eigenvalue is positive, your system is unstable.