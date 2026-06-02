![[Pasted image 20250106114712.png]]
*  for an ideal binary solution, $y_A = P_A/P_T = (x_A*P_A^V)/P_T$
* If A and B are immiscible, their mixture exerts a vapour pressure= sum of vapour pressure of individual components
* Hence the bubble point of such a mixture < boiling point of either A or B
* Process: live steam is passed through a liquid -A vapourises - leaves with steam - condensor - 2 layers - separated by decantation (if A is immiscible in steam, which is usually is)
* The substance to be distilled is usually low volatile
* Applications of steam distillation - separation of high boiling materials (decolourisation, deodourisation of vegetable oils, purification of essential oils), separation of hazardous materials, separation of thermally unstable materials
## For immiscible A in water
- A is the substance, B is water (steam)
![[Pasted image 20250106115347.png]]
* if moles of A are volatised by putting in m_B moles of steam at equilibrium:
* ![[Pasted image 20250106115552.png]]
- ![[Pasted image 20250203163103.png]] Where E is efficiency
* if the system does not separate at equilibrium: $P<P_A^V$
> [!Problem]
> Chlorobenzene is a flammable liquid and is used as a common solvent. It is proposed to purify Chlorobenzene by steam distillation at 100C and atmospheric pressure. A small scale unit is charged with 1 Liter of crude chlorobenzene containing non volatile impurities. Calculate the steam required assuming that chlorobenzene is immiscible woith water. Neglect condensation of the steam. Also estimate the boiling temperatre of the mixture

>[!FAQ] What is this image for? - even I have no clue
>```import matplotlib.pyplot as plt
import numpy as np
temp = np.arange(40,95,1)
p_a = np.exp(16.4-3485/(temp+224.87))
p_aex = 760-np.exp(18.58-3984/(temp+233.43))
plt.plot(p_a,temp,label="p_a")
plt.plot(p_aex,temp,label="p_a ex")
plt.legend()
plt.xlabel("Pressure")
plt.ylabel("temperature")
plt.show()```

![[Pasted image 20250106124010.png]]

## For A and C (nonvolatile solid) ideal binary solution, immiscible in water
- if we take x_A to be:![[Pasted image 20250203163822.png]]
- and we take rate of flow of m_b related to m_a:![[Pasted image 20250203163845.png]]
- then m_A is: ![[Pasted image 20250203163913.png]]
- (credits to BKD)

## Why
- why not just heat the substance? Why steam distillation? whats the need for steam? - because some substances are sensitive to heat and if you heat it directly to it's boiling point, bad stuff happens
- Steam and the immiscible substances form a total boiling point lower than any individual bubble point, so the temperature needed is less
## Problems
- [[Problems on Steam Distillation]]