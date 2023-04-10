X is a non-negative [[Random Variable]] with a finite mean $u = E[X]$
$$\forall a>0, P(X\geqslant a)\leqslant \frac{u}{a}$$
This is a weak inequality compared to the tighter.
$$
\begin{align}
	\mu & = \sum_{0}^{\infty}xp_{X}(x) \\
& \geq \sum_{a}^{\infty}xp_{X}(x) \\
& \geq \sum_{a}^{\infty}ap_{X}(x)  \\
& = a\sum_{a}^{\infty}p_{X}(x) \\
& = a\mathbb{P} \left\{ X\geq a \right\} 
\end{align}
$$
[[Chebyshev's Inequality]]