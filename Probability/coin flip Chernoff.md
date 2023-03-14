We flip a fair coin n times. What is the upper bound on the probability of getting at least three fourths n heads using [[Chernoff Bound]] and [[Chernoff Binomial]]
X is number of heads
$$
\begin{align*}
P(X\geqslant \frac{3n}{4}) & = P(X-\frac{n}{2}\geqslant \frac{n}{4})\\
& \leqslant e^{-2(n/4)^2/n}\\
& = e^{-n/8}
\end{align*}
$$ We subtract by $n/2$ since each coin is [[Bernoulli]] with probability 1/2 and we have n coins.