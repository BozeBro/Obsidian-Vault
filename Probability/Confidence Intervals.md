$X_{1},X_{2},\dots,X_{n}$ i.i.d $\sim X$
Want to estimate $\mathbb{E}\left[ X \right]$ [[Expectation]]
Intuition: Take the average of the values $\bar{X} = \frac{\sum_{i=1}^{n}X_{i}}{n}$
### #Confidence-Interval$\left[ \bar{X}-\delta,\bar{X}+\delta \right]$ 
We say $x\%$ confidence interval if $\mathbb{P}\left\{ \mathbb{E}\left[ X \right]\in \left[ \bar{X}-\delta,\bar{X}+\delta \right] \right\}\geqslant x\%$
Want confidence interval to be small for accurate estimation.

We can use [[Chernoff Bound]] to get Confidence-Interval
<ins>Example</ins>: p: probability a person votes for Biden.
Alg1. 
1. $X_{i}=1$ if person i will vote for Biden. 0 otherwise
2. $S_{n} X_{1}+X_{2}+\dots+X_{n}$
3. $\bar{X}=\frac{S_{n}}{n}$

Goal: Find a $\delta$, s.t. $P\left\{ p \in\left[ \bar{X}-\delta,\bar{X}+\delta \right] \right\}\geqslant 95\%$
Note, [[Tail Bounds and Applications]] and [[Random Variable]] Y
We can write the #Confidence-Interval in terms of #Tail-Bound 
$\mathbb{P}\left\{ p \geqslant \bar{X}-\delta \cap p\leqslant \bar{X}+\delta\right\} \geqslant 95\%$
$$\iff \mathbb{P} \left\{ p < \bar{X}-\delta \cup p > \bar{X}+\delta\right\}\leqslant 5\%  $$
$$
\iff \mathbb{P} \left\{ \mid\bar{X} - p \mid > \delta \right\}\leqslant 0.05 
$$
$$
\iff \mathbb{P} \left\{ \bar{X}-p>\delta \right\} + \mathbb{P} \left\{ \bar{X}-p < -\delta \right\} \leqslant 0.05 
$$
$$
\mathbb{P} \left\{ \bar{X}-p>\delta \right\}
$$

$$
= \mathbb{P} \left\{ \frac{S_{n}}{n}-p > \delta \right\} = \mathbb{P} \left\{ S_{n}-np > n\delta \right\} 
$$
$$
\leqslant e^{- \frac{2(n\delta)^{2}}{n}}=e^{-2n\delta^{2}} \text{ Pretty Binomial Chernoff}
$$
[[Chernoff Binomial]]


We know the probabilities of both must sum to be less than 5%.
Solve for delta,
$$
2e^{-\frac{2(n\delta)^{2}}{n}}=0.05
$$
We can also use [[Chebyshev's Inequality]] for this as well
$$
\begin{align}
	& \text{Pick delta s.t. } \mathbb{P} \left\{ \mid\bar{X}-p\mid \geqslant \delta \right\} \leqslant 5\% \\
	& = \mathbb{P} \left\{ \mid S_{n}-np \mid \geqslant n\delta \right\}  \\
	& \leqslant \frac{np(1-p)}{(n\delta)^{2}} \\
	& = \frac{p(1-p)}{n\delta^{2}}
\end{align}
$$
But we do not know $S_{n}$, but we can just pick the p and delta that maximizes the fraction seen above, but is still within bounds.

choice for p is $\frac{1}{2}$ and $\delta \geqslant \sqrt{ \frac{5}{n} }$ 

