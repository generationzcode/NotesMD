* for reynolds number below 2100, f = 16/Re
* For reynolds number above 2100, mile long equations follow:
* $$f = 0.079*Re^{-0.25}$$ 
* *what is this? a mile for ants?*
* The above is a Blasius relation
* This comes partly from boundary layer theory - semi empirical semi theoretical relation
> random note  - Avoid wikipedia

* $$\frac{1}{\sqrt f} =  4*log_{10}(Re\sqrt F)-0.4$$
* This is another relation. The 0.4 correction comes in from boundary layer theory. This works between 2300 and $4*10^6$ Reynolds number. Prandtl formula
* These are all ad-hoc, somehow fitted to their use
* Ladies and hopefully more ladies, I present to you, the devil's excrement (from 70 to $3.23 * 10^6$):
* $$f = \frac{2}{\psi ^ \frac{2}{\alpha+1}}$$
* $$\psi  = \frac{e^{3/2}(\sqrt 3+5\alpha)}{2^\alpha(\alpha)(\alpha+1)(\alpha+2)}$$
* $$\alpha = \frac{3}{2ln(Re)}$$
* DO NOT USE THE ABOVE IN AN EXAMINATION
* Barenblatt. No one has the slightest clue where this guy came up with this correlation from.
> Pick up a problem, any random problem, calculate f by all the correlations and see what the difference is

* $$0.046Re^{-0.2} = f$$
* For range between $5*10^5$ to $10^6$ 
* 
$$f = 0.0014+(0.125)Re^{-0.32}$$
* For range between 3000 and $3*10^6$
* To take into account roughness
* $$\frac{1}{\sqrt f} = -3.6log_{10}(\frac{6.9}{Re}+(\frac{\epsilon/D}{3.7})^{10/9})$$
* Range of the above is 40,000 to 400,000. Epsilon/D shows the roughness, and this should be between 0 and 0.05
* If the roughness is too much, replace the pipe instead of getting a new correlation

>[!Danger]
>Churchill:
>$$f = 2(\frac{8}{Re}^{12}+(A+B)^{-1.5})^{1/12}$$
>$$A=(2.457ln([\frac{7}{Re}^{0.9}+0.27\frac{\epsilon}{D}]^{-1}))^{16}$$
>$$B=(\frac{37530}{Re})^{16}$$



