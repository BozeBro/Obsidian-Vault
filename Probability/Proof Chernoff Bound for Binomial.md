We'll need #Lemma-18-5 for this proof
$$
\begin{align}
	\text{Let }&t>0,\; q = 1-p\text{ then } \\
	& pe^{tq}+qe^{-tp}\leqslant e^{t^2/8}
\end{align}

$$


$$
\begin{align}
	 X & = \sum_{i=1}^nX_{i}, \text{ where }X_{i}\sim \text{Bernoulli}(p), t> 0 \\
	\mathbb{P} \left\{ X-np\geq \delta \right\} & =  \mathbb{P} \left\{ t(X-np)\geq t\delta \right\} \text{Markov's Inequality} \\
	& \leq e^{-t\delta} \cdot \mathbb{E}\left[ e^{t(X-np)} \right]  \\
	& = e^{-t\delta}\mathbb{E}\left[ e^{t((X_{1}-p)+(X_{2}-p)+\dots+(X_{n}-p))} \right]  \\
	& = e^{=t\delta}\prod_{i=1}^{n}(p\cdot e^{t(1-p)}+(1-p)\cdot e^{-tp})  \\
 & \text{All }X_{i}\text{ are independent}\\
	& = e^{-t\delta }\prod_{i=1}^{n}(pe^{t(1-p)})+(1-p)e^{-tp} \\
	& \leqslant \prod_{i=1}^{n}(e^{t^{2}/8})\; \text{Lemma 18.5} \\
	& = e^{-t\delta + nt^2/8}
\end{align}
$$
To find minimizing t, minimize the exponent.
First look at the critical point of 
$$
-t\delta + \frac{nt^{2}}{8}
$$
$$
\begin{align}
	& \frac{d}{dt}\left( -t\delta+\frac{nt^{2}}{8} \right) = -\delta+\frac{2nt}{8} \\
	& \frac{d^{2}}{dt}\left( -t\delta+\frac{nt^{2}}{8} \right)=\frac{2n}{8} > 0
\end{align}
$$
From here we need
$$
-\delta + \frac{2nt}{8} = 0
$$
which means that $t = \frac{4\delta}{n}$
After substitution, we have $$
P(X-np\geq \delta) \leq e^{-\frac{2\delta^{2}}{n}}
$$