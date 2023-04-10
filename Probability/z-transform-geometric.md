Let $X \sim Geo(p)$ [[Geometric]]
Then, 
$$
\begin{align}
	\hat{X}(z) & = \mathbb{E}\left[ z^{X} \right] = \sum_{i=1}^{\infty}p(1-p)^{i-1}z^{i} \\
& = zp\sum_{i=1}^{\infty}(z(1-p))^{i-1} \\
&= zp\sum_{i=0}^{\infty}(z(1-p))^{i} \\
& = \frac{zp}{1-z(1-p)}
\end{align}
$$
$$
\begin{align}
	\hat{X}(z) & = \frac{zp}{1-z(1-p)} \\
\mathbb{E}\left[ X \right] & = \frac{d}{dz}\left( \frac{zp}{1-z(1-p)} \right)\mid_{z=1}  \\
& = \frac{p}{(1-z(1-p))^{2}}\mid_{z=1} = \frac{1}{p} \\

\end{align}
$$
