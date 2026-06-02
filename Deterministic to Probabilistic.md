- Lets take an equation: $$\frac{dN}{dt} = r_mN(\frac NA-1)(1-\frac NK)$$
=> $$\frac{dN}{Ndt} = r_m(\frac NA-1)(1-\frac NK)$$
=> $${dN} = r_mN(\frac NA-1)(1-\frac NK)+\sigma N(t)dW(t)$$
where $dW(t)\propto N(0,dt)$
=>$$N(t+dt)-N(t) = r_mN(t)(\frac {N(t)}A-1)(1-\frac {N(t)}K)dt+\sigma N(t)(W(t+dt)-W(t))$$
=>$$N(t_0+dt) = N(t_0)+r_mN(t_0)(\frac {N(t_0)}A-1)(1-\frac {N(t_0)}K)dt+\sigma N(t_0)(W(t_0+dt)-W(t_0))$$
- Sigma here is the intensity of the noise, dW(t) is the white noise component
- $$N(t_0+dt) \propto N(\mu(t_0), \sigma^2N(t_0)^2dt)$$
- The N above and the N in the equation are separate. The N with two parameters is the normal distribution with mean and variance as the parameters
- 