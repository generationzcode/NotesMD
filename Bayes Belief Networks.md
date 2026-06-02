>  Every example of this everywhere seems to use rain, sprinklers and wet grass. Either no one in the field understood it, or this concept just makes people yearn the outdoors

- So this is all built on bayes theorem, a way to update beliefs on learning of new evidence (or conditions):
- $$P(A|B) = \frac{P(A)*P(B|A)}{P(B)}$$
- The new evidence in the above case is the fact that A is occurring when B has already occurred, requiring the belief to be updated if it is to be accurate
- We can exploit this in massive networks of thousands of probabilities to learn of the probabilities of very niche events composed of many conditions. These networks travel up and down the various events and conditional probabilities calculated to get the final probability
## DAG
- Bayesian Belief Networks (BBNs) use Directed Acyclic Graphs (DAGs) to represent events as below:
- ![[Pasted image 20250318150327.png]]
- The above DAG shows that the event of grass being wet depends on both the sprinkler and the rain, the event of the sprinkler turning on depends on it raining or not and that the rain node is the "base" node, which isn't dependent on anything, keeping the BBN acyclic
- If the BBN were to get cyclic, it would cause logical paradoxes. A->B->C->A implies that the occurrence affects the occurrence of A, or the occurrence of A influences the occurrence of B, which influences A - breaking causality
- ![[Pasted image 20250318150653.png]]
- The above picture really sells the idea well - the lower you go, the more dependencies you get, more conditions
- Now if I want to now the probability of the sprinkler having switched on if the grass was wet, I can. you would take the probability of the sprinkler switching on (prior belief), multiply is with the probability of the grass being wet if the sprinkler was on (the first two rows after computing the joint probabilities), divide it by the probability of the grass being wet