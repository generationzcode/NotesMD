> This builds little from [[Taxonomy]], but not too much

- The language in which we'll make our generalizations is the hypothesis language
- Generalizations are consistent with the training samples if and only if there are no errors in matching
- The hypothesis language has many effects on the outcome. If the language is represented in the form of graphs, the complexity is exponential, but if it's a feature vector with ranges and such, it's linear complexity
- "More specific than" relation between hypotheses -> Between two generalizations, if one has instances that are a proper subset of the other's instances, it's more specific than. This relation helps us organize the search for hypotheses better, and as such, methods of computing this relation without iterating through all possible instances are required, causing a constraint on hypothesis language
- POSET - a partially ordered set, basically an ordered set, but not all elements are comparable
## Generalization strategies
- Ways to get the most general hypothesis 
- "Data driven" - The training data is traversed and hypotheses are learned from there
- "Generate and test" - The possible hypotheses are searched and instance space is tested against. Hypotheses generated are independent of the training data, once they are generated, they are tested against data to check for acceptability of node. If not, they are pruned
- Generate and test are more resistant to individual instance error in data, however, cannot be used to keep training online
- Depth First Search (Data Driven) - generates a "current best hypothesis" from the frst training sample, then keeps altering it over the other instances, always checking back with the elapsed instances whether the CBH works, if not, it backtracks and re-alters. Very computationally expensive
- Breadth first search (data driven) - generates a set of extremely specific hypotheses and builds up generalizations from there
- Version space (data driven) - generates an extremely general and an extremely specific set of hypotheses, anything that lies in between the two is in the version space.
- 