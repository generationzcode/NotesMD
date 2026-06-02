>[!faq] Confused...
>Why did BSL use $s$ instead of $t$ in the $v_z(t)dt$ part? What is $s$ and why is velocity a function of it? What are we integrating over?
- $$\bar v_z = \frac{1}{t_0}\int^{t+\frac{1}{2}t_0}_{t-\frac{1}{2}t_0}{v_z(t)dt}$$
- that's the time smoothed velocity in $v_z = \bar v_z +v_z'$. $v_z'$ is the fluctuation 
-  $\bar v' = 0$, obviously... (average of fluctuation over time)
- Using [[Equation of motion]] to write out one for turbulent flow:
- $$\delta \rho\bar v/\delta t = -\nabla\bar p-\nabla . \rho \bar v \bar v - \nabla.(\tau^v+\tau^t)+\rho g$$ in tensor form
- Now in cartesian form, lets take the x component EoM:
- $$\begin{aligned} 
\frac{\delta}{\delta t}\rho(\bar v_x+v_x') = -\frac{\delta}{\delta x}(\bar p+p')-(\frac{\delta}{\delta x} \rho(\bar v_x+v_x')(\bar v_x + v_x')+ \frac{\delta}{\delta y} \rho(\bar v_y+v_y')(\bar v_x + v_x')\\
+\frac{\delta}{\delta z} \rho(\bar v_z+v_z')(\bar v_x + v_x'))+\mu \nabla^2(\bar v_x+v_x')+\rho g_z
\end{aligned}$$
- This simplifies to give:
- $$\begin{aligned} 
\frac{\delta}{\delta t}\rho(\bar v_x) = -\frac{\delta}{\delta x}(\bar p)-(\frac{\delta}{\delta x} \rho(\bar v_x)(\bar v_x)+ \frac{\delta}{\delta y} \rho(\bar v_y)(\bar v_x)+\frac{\delta}{\delta z} \rho(\bar v_z)(\bar v_x))-\\ (\frac{\delta}{\delta x} \rho(\overline{ v_x' v_x'})+ \frac{\delta}{\delta y} \rho(\overline{ v_y' v_x'})+\frac{\delta}{\delta z} \rho(\overline{ v_z' v_x'}))\\+\mu \nabla^2(\bar v_x)+\rho g_z
\end{aligned}$$
- Now the second convective momentum transfer set of terms is called the turbulent momentum flux
- $$\tau_{xx}^t =\rho \overline{v_x'v_x'}$$ $$\tau_{yx}^t = \rho \overline{v_y'v_x'}$$ $$\tau_{zx}^t =\rho \overline{v_z'v_x'}$$
- These are known as the Reynold's stresses, and in [[Turbulent Momentum Flux]], we'll talk more about different aspects of it
- The part of the EoM with a $\mu$ and a $\nabla^2$ is the time smoothed velocity part. It's just viscous momentum flux
>[!FAQ] Confused
>I'll be honest, I think we jumped step by just time smoothing. I don't get the reason why the correlations $$$\overline{v_x'v_x'}$$ are time smoothed. Must be some simple reason I'm not getting. Majikthise and Vroomfondel seem ever smarter now. Maybe I'm just too trained to understand some really smart stuff. 
>
>I also have absolutely no clue what the last paragraph of BSL states here. How do reynolds stresses have $\overline{v_iv_jv_k}$? I just derived the equation and it doesn't! What do you mean they come into play in higher and higher orders? An older edition tried to explain more of this in it's last two pages (of the chapter), but to blind eyes. I just cannot understand what they're trying to say.


- Okay, so a good reason why reynolds stresses cant be used really is because you have what? 4 equations for EoC and 10 variables with all the reynolds stresses and such. Impossible to solve. Thanks to my professors ppt!