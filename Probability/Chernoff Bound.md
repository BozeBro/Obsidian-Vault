Derived from Markov's Inequality
$$
\begin{align*}
P(X\geqslant a) & = P(tX\geqslant ta)\\
&= P(e^{tX}\geqslant e^{ta})\\
&\leqslant \frac{E[e^{tX}]}{e^{ta}}
\end{align*} $$
So we know 
$$P(X\geqslant a)\leqslant min_{t>0}\frac{E[e^{tX}]}{e^{ta}}$$
Chernoff is stronger than [[Chebyshev's Inequality]] Since we look at all the [[kth Moment]] of the random variable instead of the 2nd moment ([[Variance]])
If looking at $P(X\leqslant a)$ then look at any $t<0$ 

See [[Chernoff Poisson]]
[[Chernoff Binomial]]
