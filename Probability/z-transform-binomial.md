$$
\hat{X}(z) = (zp+(1-p))^{n}
$$

$$
\begin{align}
	\hat{X}(z) = \mathbb{E}\left[ z^{X} \right] & = \sum_{i=0}^{n} {n \choose i}p^{i}(1-p)^{n-i}z^{i}  \\
& = \sum_{i=0}^{n}{n\choose i}(zp)^{i}(1-p)^{n-i} \\
& = (zp + (1-p))^{n}
\end{align}

$$
Since we have [[Z-Transforms#^abf9aa]]
then if $X\sim Bin(n,p)$ and $Y\sim Bin(m,p)$
$Z = X + Y\sim Bin(n+m, p)$
$$
\begin{align}
	\hat{Z} & = \hat{X}\hat{Y} \\
& = (zp+(1-p))^{n}\cdot (zp+(1-p))^{m} \\
& = (zp+(1-p))^{m+n}
\end{align}
$$

