Want to do analysis through function calls
Two Simple Approaches
1. [[Default Assumptions]]
2. [[Annotations]]
Make sure to consider local and global variables
Make conservative assumption about both.
[[lattice]] value $L_{g}$ describes global varaibles
$$
\begin{align}
	& f\left[ x := g(y) \right] (\sigma) = \sigma \left[ x\to L_{r} \right] \left[ z \to L_{g}\mid z\in \text{ Globals } \right] \\ &
\text{error if }\sigma(y)\not\sqsubseteq L_{a}\vee \forall z \in \text{ Globals } : \sigma(z) \not\sqsubseteq L_{g}) \\
	& f\left[ \text{Return x} \right] (\sigma) = \sigma  \\
	&\text{ error if }\sigma(x)\not\sqsubseteq L_{r}\vee\forall z \in \text{ Globals } : \sigma(z) \not\sqsubseteq L_{g}\\
\end{align}
$$
## Interprocedural Control Flow Graphs
![[Screen Shot 2023-03-15 at 12.49.34 PM.png]]


A better way is use to [[Context Sensitive Analysis]]
