Let $m \geqslant 2n \ln n$
We first want to show for any $B_{i}$, 
$$
\mathbb{P} \left\{ B_{i} \geqslant e \alpha \right\} \leqslant \frac{1}{n^{2}}
$$
Then with that result, we can use [[union bound]]
$$
\mathbb{P} \left\{ \text{Arb bucket has } \geqslant e \alpha \text{balls} \right\} \leqslant \sum_{i=1}^{n} \frac{1}{n^{2}} = \frac{1}{n}
$$
Thus, $$
\mathbb{P} \left\{ X < e \alpha \right\} > 1 - \frac{1}{n}
$$
Start with $\alpha = \frac{m}{n} \geqslant 2 \ln n$
Do we use #Theorem18-4 or #Theorem18-6 ?
We'll use [[Sometimes Stronger Chernoff]] since $\alpha$ is on the order of $\ln n$ not $n$
Suppose $1 + \epsilon = e$ ($\epsilon = e - 1 > 0$) and $\mu = \alpha > 1$
$$
\begin{align}
	  \mathbb{P}\left\{ B_{i} \geqslant e \alpha \right\} & = \mathbb{P}\left\{ B_{i} \geqslant (1 + \epsilon)\mu \right\}  \\
& < \left( \frac{e^{\epsilon}}{(1 + \epsilon)^{1 + \epsilon}} \right)^{\mu} \\
& = \left( \frac{e^{e - 1}}{e^{e}} \right)^{\alpha} \\
& = (e^{-1})^{\alpha} \\
& < (e^{-1})^{2 \ln n} \\
& = (e^{\ln n})^{-2} \\
& = \frac{1}{n^{2}}  
\end{align}
$$