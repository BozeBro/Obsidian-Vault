X is a  [[Random Variable]] with a finite mean $\sigma_X^2=u = E[X]$ and finite [[Variance]]
Then $$\forall a>0\, P(\mid X-u\mid\geqslant a)\leqslant \frac{Var(X)}{a^2}$$
$$
\begin{align}
	\mathbb{P} \left\{ \mid X - \mu \mid \geq a \right\}  & = \mathbb{P} \left\{ (X-\mu)^{2} \geq a^{2} \right\}  \\
& \leq \frac{\mathbb{E}\left[ (X-\mu)^{2} \right] }{a^{2}} \\
& = \frac{Var(X)}{a^{2}}
\end{align}
$$
Chebyshev is stronger than [[Markov's Inequality]] since we take into account [[Variance]]. Equivalent definitions below.
$$P(\mid X-u\mid\geqslant a\sigma_X)\leqslant \frac{1}{a^2}$$
$$P(\mid X-u\mid\geqslant aE[X])\leqslant \frac{C_X^2}{a^2}$$
where $C^2_X$ is the [[squared coefficient of variance]] of X
In cases where we are trying to see the odds of being better than some function of n,
[[Chernoff Bound]] will be a better bound since it decays with higher n (only when seeing if greater than a function of n)
#stochastic-dominance
$$
\mathbb{P} \left\{ X > i \right\} \geq \mathbb{P} \left\{ Y > i \right\}\, \forall i
$$
Then $X \geq_{st} Y$

