> many components, we assume ideality - much simpler...

- if we take $\alpha_{ij}$ as the relative volatility for each component, with respect to a reference volatility j - 
- The component balance for i and j, building from [[Batch Distillation of Binary Mixtures]]:$$dL_i = y_{Di}dL$$, $$dL_j = y_{Di}dL$$
- => $$\frac{dL_i}{dL_j} = \frac{y_{Di}}{y_{Dj}} = \alpha_{ij}\frac{x_i}{x_j} = \alpha_{ij}\frac{L_i}{L_j}$$
- on integrating: 
![[Pasted image 20250204221211.png]]
- On repeating this with all the other components with respect to j, or i: ![[Pasted image 20250204221239.png]]
- this with the fact that totality of x has to be 1, can solve a batch problem
- I'll do the examples later
## Why?
>[!Warning] Unstable Information
- binary math looked so much tougher than this - why? why isn't this equally complicated?
- in binary, the deviation starts right from the dLx, it has like 2 degrees of freedom basically - how much the W is and equilibrium data, from that composition is defined, but multicomponent, needs atleast one component's start and end composition, W, equilibrium data of all components with the reference
- I need to come back to this later and verify this whole degrees of freedom thing... But this is the general vibe here
## Problems
- [[Problems on batch distillation of multicomponent mixtures]]