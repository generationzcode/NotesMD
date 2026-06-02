- Drawn upside down, from the top down
- nodes represent features, edges represent feature values/intervals
- leaves represent outcomes
- Classification tree leaves are of classes and regression leaves are of intervals or real number
- The first split is called the root split, then child splits
- ![[Pasted image 20250318143204.png]]
## Learning
> Symbolic AI, using weak theories in inductive learning

- To make a tree, we need to choose features at nodes to discriminate at every level. This is a problem to solve
- The order of instances used to train the tree shouldn't affect it's growth
- Purity or homogeneity at nodes and leaves of decision trees mean the amount of mixing of classes (less mix -> higher purity)
- To choose which feature to separate at each node, we use "information theoretic measures"
- Information gain based on entropy (information entropy, not [[Entropy]]) - measures how well a given feature discriminates data. An example:
- ![[Pasted image 20250318222544.png]]
- total entropy of dataset: ![[Pasted image 20250318222615.png]]
- entropy after splitting at outlook:
- sunny has 2 yes, 1 no which is 0.918, etc
- ![[Pasted image 20250318222712.png]]
- this, repeated for other fields, reveals information gain (0.954-0.688) is maximum for splitting at outlook and this thats where we should split

- Gini Impurity - its information entropy except -p* log p is replaced by $1-p^2$ kinda
- ID3 is a way to make decision trees by a greedy, top down approach, maximising information gain at each node
- TDIDT is a general framework of which ID3 is a part for making decision trees
- Boosting - ensemble technique (many trees), trees trained sequentially, correcting the errors of the tree before it
- Bagging - ensemble technique, trees run parallel