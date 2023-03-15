
$$
X=
\begin{cases}
x_0, & \text{with prob }p_0\\
x_1& \text{with prob }p_1\\
\ldots \\
x_k& \text{with prob }p_k
\end{cases}
$$

### Algorithm
1. Arrange $x_0,\ldots, x_k$ s.t. $x_0<x_1<\ldots<x_k$
2. Generate $u\in U(0,1)$ 
3. 
	1. If $0<u\leqslant p_0$, then output $x_0$
	2. If $p_0 < u p_0 +p_1$, then output $x_1$
	3. $\ldots$
	4. If $p_{k-1} < u<=p_{k-1}+p_k$, then output $x_k$
Whatever boundary we are in, output the lefthand side variable
Only practical when we have a closed form of the $P(X\leqslant a)$ function
See [[inverse transform method]] and [[Continuous inverse transform method]] for more inverse information

