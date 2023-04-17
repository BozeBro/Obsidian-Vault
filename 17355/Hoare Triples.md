$$
P\wedge S \implies Q
$$
P is precondition, S is code, Q is post condition
![[Verification.pdf]]

Example Hoare Rule for let rule
$$
\begin{align}
	& \left[ x / x' \right] \left[ e / x' \right] VC\left(S, \left[x' / x\right] Q \right) \\
& \left[ e / x' \right] VC\left(\left[ x' / x \right] S, Q\right) 
\end{align}
$$
 

