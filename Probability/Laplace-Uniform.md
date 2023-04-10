[[Uniform]]
$X \sim \text{Uniform}(a,b),\; a,b \geq 0$
$$
\begin{align}
	\tilde{X}(s) & = \int_{0}^{\infty} e^{-st}f_{X}(t) \, dt \\
& = \int_{a}^{b} e^{-st} \frac{1}{b-a} \, dt \\
& = \left( \frac{-e^{-sb}}{b}+ \frac{e^{-sa}}{s} \right) \frac{1}{b-a} \\
& = \frac{e^{-sa}-e^{-sb}}{s(b-a)} 
\end{align}
$$
