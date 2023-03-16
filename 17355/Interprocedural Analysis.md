Want to do analysis through function calls
Two Simple Approaches
1. [[Default Assumptions]]
2. [[Annotations]]
Make sure to consider local and gloval variables
Make conservative assumption about both.
[[lattice]] value $L_{g}$ describes global varaibles
$$
\begin{align}
	& f\left[ x := g(y) \right] (\sigma) = \sigma \left[ x\to L_{r} \right] \left[ z \to L_{g}\mid z\in \text{ Globals } \right] \\ &
\text{error if }\sigma(y)\not\sqsubseteq L_{a}\vee \forall z \in \text{ Globals } : \sigma(z) \not\sqsubseteq L_{g}) \\
	& f\left[ \mathrm{Re}turn x \right] (\sigma) = \sigma  \\
	&\text{ error if }\sigma(x)\not\sqsubseteq L_{r}\vee\forall z \in \text{ Globals } : \sigma(z) \not\sqsubseteq L_{g}\\
\end{align}
$$
## Interprocedural Control Flow Graphs
![[Screen Shot 2023-03-15 at 12.49.34 PM.png]]

A better way is use to Context-Sensitive Analysis
## Context Sensitive Analysis
When analayzing function calls, have analysis results reflect different analysis results that are passed in.
### Inlining can work since it keeps the context but only for non recursive functions
**Solution #1**, build a summary for each possible input

Problems when there is recursion since inputs will change, since we can have no termination if we Top propogates or not be able to create a summary that terminates. If we treat recursion as a loop, than we can do analysis accurately.


![[Screen Shot 2023-03-15 at 1.00.35 PM.png]]![[Screen Shot 2023-03-15 at 1.00.28 PM.png]]![[Screen Shot 2023-03-15 at 1.00.16 PM.png]]

For function calls, if multiple return statements, results are joined together.