Different from heuristic techniquest. 
Construct repair constraint that patched code should satisfy. Treated as a program to be synthesized. We can run Symbolic execution to ensure properties about a function. 
formulation of the constraint is key, not the mechanism for solving it. Schematic follows
$$
\begin{align}
	& \text{for } & \text{test t} \in \text{test-suite T} \\ & & \text{computer repair constraint} \\
& \text{synthesize} & \text{e as solution for }
\end{align}
$$
where T is the test-suite to see correctness. 
Constraints calcualted with symbolic execution. Generally constriant made from path condition tot get to a condition. 
Runs into scaling problems. 
Try [[angelic values]] from inferred for patch locations. It is a When angelic values made for each failing test, we can perform program syntehsis. See [Angelix Tool](http://angelix.io/)
Angelic values can obtained through symbolic execution or search.