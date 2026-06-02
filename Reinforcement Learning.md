> Humanlike

- ![[Pasted image 20250319114152.png]]
	`` The above image pretty much sums up whats going on, so I won't waste our time explaining it ``
- ==Terminal state - end state desired for the agent (eg. winning the chess match)==
- Policy - strategy basically
- Transition probability function - the probability that the environment will transition to a particular state after a particular action (eg. car turns right, skids or not)
- Episode - A.K.A epoque (not epoch?). A series of states and actions that results in a terminal state
- Discounted reward - a reward discounted for the rewards expected in the future (so as to prevent the agent from being too greedy)
- Return - discounted rewards from an episode
- If the transition probability function and the reward function are well defined for the entire environment states, then its no longer an RL problem, its a DP problem
- Dynamic programming divides a big problem into smaller subproblems and optimizes
- Dynamic programming MDPs are solved by optimizing bellmans equations
- theres also some stuff on POMDP, where the agent is governed by an MDP, but cannot observe the underlying states directly (????)
## Learning Methods
- Passive learning - agent doesnt interact with the system, just observes and understands the consequences
- Active learning - agent interaction with environment affecting outcomes
- When we use a DP method, we use off policy planning, where the agent plans without interacting with the world
- On policy planning is when the agent plans while interacting with the environment when the total model of the environment isn't possible to simulate
- Exploration vs Exploitation, basically innovation vs exploitation kinda. If you explore too much you won't get any rewards, but if you exploit too much, greedily, you'll never find the global maxima. This is a tradeoff we must make
-  Model based algorithms - they learn a model of the environment then solve a planning problem for policy
- Model free algorithms - no model, eg. Q-learning
### Model Based
#### Adaptive Dynamic Programming
- Completes the partially known MDP and then uses dynamic programming and evaluates the value function (that bellman thing)
### Model Free
#### Monte Carlo
- for some reason the title in the ppt says model based, but I'm pretty sure it's model free
- it's an off policy method
- It just averages the returns from each episode containing a specific state to get the value of that state
#### Temporal Difference Learning
- So you have a bunch of states and the agent has estimates of the values of each state (value of a state is the discounted total rewards after it till terminal state)
- When an agent moves from one state to another, the value of the state its moving from can be calculated by:
- ![[Pasted image 20250319165803.png]]
- where gamma is the discount factor, alpha is the learning rate, R is the observed reward for the action
- The value after alpha in the equation above ($R_{t+1}+...-V(s_t)$) is called the temporal difference (TD) error
#### Q-Learning
- A variant of TD learning
- It's legit the same as TD learning, everything,except the V value is replaced by Q, which takes into account action as well as state, Q(s,a)
- so you have a different Q value for every state for every action taken by the agent in that state to get to another state