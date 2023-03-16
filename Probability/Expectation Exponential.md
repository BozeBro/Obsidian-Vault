Expectation is $\frac{1}{\lambda}$
$$
\begin{align}
	\mathbb{E}\left[ X \right] & = \int_{0}^{\infty} x f_{X}(x) \, dx \\
    & = \int_{0}^{\infty} x\lambda e^{-\lambda x} \, dx  \\
    & = \lambda \left[ -\frac{xe^{-\lambda x}}{\lambda} + \int_{0}^{\infty} \frac{e^{-\lambda x}}{\lambda} \, dx \right] \\
 & =   \lambda \left[ -\frac{xe^{-\lambda x}}{\lambda} - \frac{e^{-\lambda x}}{\lambda^{2}} \right]_{0}^{\infty} \\
	& = 0 - \lambda \left[ 0 - \frac{1}{\lambda^{2}} \right]  \\
	& = \frac{1}{\lambda}
\end{align}
$$

[[Exponential]]
[[Expectation]]
