> Weak stuff

- we have some background knowledge, but are mostly required to derive rules from the data instead of generalizing them or explaining their application
- funnily enough this is covered in "generate and test" strategies in [[Generalization as Search]]
- Elements of the algorithm: initialize a set of hypotheses, delete a hypothesis from the set, expand the hypothesis using generalization or specialization rules, new hypothesis added to set, set of hypotheses is pruned for bad hypotheses, keep repeating the above till stop criterion is met
- Sufficiency - hypothesis covers all the positive examples
- Necessity - all the positive examples are not covered without hypothesis (??)
- Weak consistency - hypothesis does not contradict any element of domain theory
- Strong consistency - hypothesis is not consistent with the negative examples

## Generalization through Inverse Resolution
- resolution is basically deduction from facts and rules
- so this uses a positive instance not covered to expand a rule (generalization)
- It goes from the result to the rule upwards
- ![[Pasted image 20250319112633.png]]
## Specialization through $\Theta$ - subsumption
- If we have two clauses, and one theta subsumes the other, it's more specific
- ![[Pasted image 20250319113620.png]]