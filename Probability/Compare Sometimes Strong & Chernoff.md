$X \sim Bin\left(n, \frac{1}{2} \right)$ $p_{i} = p = \frac{1}{2}, \forall i$
Want to find $\mathbb{P}\left\{ X \geqslant \frac{3}{4}n \right\}$
#Theorem18-4 [[Chernoff Binomial]]
$P\left\{ X - \frac{n}{2}\geqslant \frac{n}{4} \right\}\leqslant e^{- \frac{2(n/4)^{2}}{n}} = e^{- \frac{n}{8}}$
#Theorem18-6 [[Sometimes Stronger Chernoff]]
$$
\begin{align}
	& P\left( X \geqslant \frac{3}{4}n \right) \\
	& = \mathbb{P} \left\{ X \geqslant \left( 1 + { \frac{1}{2}}\right) \frac{n}{2} \right\}  \\
	& \leqslant \left( \frac{e^{1/2}}{(1.5)^{1.5}} \right)^{n/2} \\
	& = 1.54^{- \frac{n}{2}}
\end{align}
$$
