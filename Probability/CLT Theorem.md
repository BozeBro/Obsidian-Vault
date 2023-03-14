[[Central Limit Theorem]]

Let $X_1,X_2,\ldots,X_n$ be i.i.d [[Random Variable]] with commean [[Expectation]] $u$ and finite [[Variance]] $\sigma^2$ and we define
$$S_n=\sum_{i=1}^nX_i \text{ and } Z_n=\frac{S_n-nu}{\sigma\sqrt{n}}$$
Then, $Z_n$ converges to the [[Standard normal]], N(0,1) as $n\to\infty$.
$$\forall z\; lim_{n\to\infty}P(Z_n\leqslant z) = \phi(z) = \frac{1}{\sqrt{2z}}\int_{-\infty}^{z}e^{-x^2/2}dx$$
See [[Normal Distribution]] for more information on normal distributions.
Note, u, and $\sigma$ denote the distribution of $X_i$, not $S_n$ 

Good for approximating, no specification if upperbound or lower bound
See [[inequalities]] to see how to bound [[Random Variable]]