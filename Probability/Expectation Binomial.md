Given n [[Bernoulli]] variables with probability p, and X is Bin(n,p)
See [[Expectation Bernoulli]] on how to get [[Expectation]] of Bern
$$
\begin{align}
	 
	\end{align}
$$
$$
\begin{align}
	X_{i}&\sim \text{Bernoulli(p)} \\
	X & = \sum_{i=1}^{n}X_{i} \\
	\mathbb{E}\left[ X \right]  & = \mathbb{E}\left[ \sum_{i=1}^{n}X_{i} \right]  \\
	& = \sum_{i=1}^{n}\mathbb{E}\left[ X_{i} \right]  \\
	& = \sum_{i=1}^{n}p \\
	& = np
\end{align}
$$