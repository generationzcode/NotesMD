Make yourself a 2D particle simulation. The particles must woosh about and kick each other around, occasionally sit by each other for a chat, a chai. So, gang, there are N particles in the mix. They each have a position (x,y) and a velocity (vx,vy). Acceleration of the particles depends on the sum of pairwise interaction forces between the particles and others near it, friction (to simulate a medium, you'll see why later). The interaction forces will have their attraction and repulsion components. The equations are given below. You are to build a set of differential equations or **invent a new mathematical technique**(joke) to see how the particles in this system behave over time. 

$$\frac{dr_i}{dt} = v_i$$
$$m\frac{dv_i}{dt} = \Sigma_{j\not=i} F_{ij}-\gamma v_i$$
$F_{ij}$ is a bit of an emo function. So we must define 2 radii for particles: $r_0$, $r_1$, where the first is the radius below which repulsion is the controlling force and $r_1$ is the radius after which no force is applicable between that particle and the rest
- When the distance between two particles, $r_{ij}<r_0$: $$F_{AB} = G_{KL}A(1-\frac{r}{r_0})$$
- $r_1>r_{ij}>r_0$: $$F_{ij} = -G_{KL}B(1-\frac{r-r_0}{r_1-r_0})$$
- if its more than r1, you can assume the force is 0

Very importantly, pay close attention to what $G_{KL}$ is. It's an interaction parameter between classes of particles. You can have as many classes of particles in your mixtures (keep more than two to see exciting stuff). K and L were just filler letters for this. 

Keep in mind that the forces must be in the vector direction of $r_{ij}$.

To talk a little more on the attraction parameter. They show how much different classes of particles attract and repel each other - basically how much they interact with each other.  It's easy to visualise this as a matrix of interaction parameters: ![[Pasted image 20260105002156.png]]
It must, then be a symmetric matrix since the pairwise interactions between any two particles must be the same (otherwise you break an array of physics laws)


Your task is to make this simulation of particles, and make a video or GIF animation of it using python. If I were you, and I wasn't using something like P5JS and didnt know python drawing libraries like the back of my hand, I'd just plot it and animate the plot.

Enjoy.

ALSO MAKE WALLS!!!
## Now interpret your creation and how it relates to real life:
Once you actually run this simulation, it's beautiful. Simply breathtaking. You'll notice that sometimes the particles form complex looking clumps and move about in very pretty, very ordered manners. If this is a simulation of particles that seemingly follows the laws of physics, then WHY? WHY isn't it absolutely random, completely chaotic? We all know that a fundamental law of the universe is that entropy increases. Why doesn't it become more chaotic? (no need to answer this (you can if you want though...), just ponder upon it and maybe do a google search after the contest)

From a thermodynamic point of view, the chemical potential of a component measures the free energy cost of removing one particle from its current environment and placing it elsewhere, such as into a vapour phase. In the simulation, this is reflected by how deep the effective potential well of a particle is due to its neighbours and how constrained it is by packing. Strong cross interactions that stabilise a particle lower its chemical potential relative to an ideal mixture, while weaker cross interactions or poor packing raise it. Even though all particles may attract each other, what matters is whether the mixed environment stabilises a particle more or less than expected from ideal mixing.

With this in mind, explore how changing the off diagonal elements of the interaction matrix alters the structures you see and the ease with which particles escape from dense regions into low density regions. When cross interactions are strong, particles become more tightly bound within mixed clusters and escape events are rare. When cross interactions are weak, particles feel less stabilised by unlike neighbours and are more likely to leave the liquid like region. Based on what you observe, ask yourself: how would the tendency of each component to vaporize change as the cross interaction strength is varied, and how does this connect to the idea of activity coefficients being greater than or less than one in real liquid mixtures?


Notes: 
- While I really want to include funny and cool images in this question, I won't. The video you'll generate yourself is more than enough stimulation