> Different to rules based systems in the sense they don't have rules, but cases stored, that can be adapted to different uses and handle more complex, unstructured type of problems

- uses cases to solve problems.
- Has 4 modes of operation: Retrieve, Reuse, Revise and Retain
![[Pasted image 20250319174333.png]]
## Loop
### Retrieve 
- Find a small number of cases from the knowledge most similar to the current case
- Can be retrieved using kd trees, discrimination networks
### Reuse
- If the current case is identical to the one retrieved, the same solution is used, else it is adapted
- Transformational adaptation: modifies the previous solution using operators specific to the the domain of the system
- Derivational Adaptation: Reuse the method that generated the original solution to the solution here
### Revise
- Feedback from the usage of the solution can be used to revise it
### Retain
- Store the final solution in the knowledge base

## Conclusion
- Most learning methods make explicit generalizations during training time, eager generalization
- CBR makes generalizations during testing time (as shown in the loop), this is obvious, as there is **no** training time for a CBR, its all testing