
- $$\frac{\delta P}{\delta z} = \mu(\frac{\delta}{r\delta r}(\frac{r\delta(v_z)}{\delta r}))+\rho g_z$$
- - $$\int\frac{\delta P}{\delta z}-\rho g_z= C_1 $$
- considering the $\rho g_z$ as a part of the pressure:
- $$P = C_1z+C_2$$
- at z=0, $P = C_2= P_0$ and at z=L, $P = P_L$
- $$P = \frac{P_L-P_0}{L}z+P_0$$
- Now, on integration of LHS:
- $$\frac{\delta}{\delta r}(r\frac{\delta v_z}{\delta r}) = C_1r/\mu$$
- Integrating once: $$\frac{\delta v_z}{\delta r} = \frac{C_1r}{2\mu}+C_3/r$$
- Putting r = 0 at the centreline, the velocity gradient = infinity ($\infty$), therefore $C_3 = 0$
- $$\frac{\delta v_z}{\delta r} = \frac{C_1r}{2\mu}$$
- Integrating again:
- $$v_z = \frac{C_1r^2}{4\mu}+C_4$$
- at $r = R_w$, $v_z = 0$
- $$0 = \frac{C_1R_w^2}{4\mu}+C_4$$
- $$-\frac{C_1R_w^2}{4\mu}=C_4$$
- Thus the velocity profile is
- $$v_z = \frac{C_1r^2}{4\mu}-\frac{C_1R_w^2}{4\mu}$$
## Differential Flow Rate
>"quit when you're up or something of that sort" - advice that we are definitely not following here

- $$dQ = v_Z*rdrd\theta$$
- This is obvious so I won't elaborate
- $$dQ = \frac{C_1}{4\mu}(r^2-R_w^2)rdrd\theta$$
- on integrating:
- $$Q = \frac{C_1}{4\mu}\int^{2\pi}_0\int^{R_w}_0(r^2-R_w^2)rdrd\theta$$
- $$Q = \frac{2\pi C_1}{4\mu}\int^{R_w}_0(r^2-R_w^2)rdr$$
- $$Q = -\frac{\pi C_1R_w^4}{8\mu}$$
- $$Q = \frac{\pi R_w^4}{8\mu}(\frac{\Delta P}{L})$$
- $$v_{avg} = \frac{R_w^2}{8\mu}(\frac{\Delta P}{L})$$
## Annular flow
- $$\frac{\mu}{r}(\frac{\delta}{r\delta r}(r\frac{\delta v_z}{\delta r})) = \frac{\delta P}{\delta z}-\rho g_z = C_1$$
- you can solve this by taking the two boundary conditions being no slip at the walls OR taking one no slip condition and knowing where the velocity gradient is 0.
- $$\frac{C_1r^2}{2\mu}+C_2 = r\frac{\delta v_z}{\delta r}$$
- $$C_1r/2\mu+C2/r = \frac{\delta v_z}{\delta r}$$
- $$\frac{C_1r^2}{4\mu}+C_2\ln r +C3= v_z$$
- $$C_1R^2/4\mu+C_2lnR + C_3= 0$$
- $$C_1(R_i^2-R^2)/4\mu+C_2ln(R_i/R) = 0$$
- $$C_2 = \frac{C_1(R_i^2-R^2)}{4\mu \ln (R_i/R)}$$
- so velocity profile in annulus:
- $$C_1r^2/4\mu+\frac{C_1(R_i^2-R^2)}{4\mu \ln (R_i/R)}lnr -C_1R^2/4\mu-\frac{C_1(R_i^2-R^2)}{4\mu \ln (R_i/R)}lnR= v_z$$
- to find where the velocity gradient is 0:
- $$\sqrt \frac{(R^2-R_i^2)}{2\ln (R_i/R)} = R_{\frac{\delta v_z}{\delta r}=0}$$
- 