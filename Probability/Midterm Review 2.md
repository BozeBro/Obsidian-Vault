[[Z-Transforms]], specifically [[Z-Transforms#^93e98f]]
Laplace transforms we know
1. [[Laplace-Uniform]]
2. [[Laplace-Exponential]]
3. [[Laplace-Random-Sums]]
[[Poisson Process]]
[[Poisson Splitting]]
[[Poisson Process#^b01df0]]
1. [[1st Poisson Process Def]]
2. [[2nd Poisson Process Def]]
Given $X_{1} \sim Exp(\lambda_{1}, X_{2} \sim Exp(\lambda_{2})), X_{1}\bot X_{2}$
$$
\mathbb{P} \left\{ X_{1} < X_{2} \right\} = \frac{\lambda_{1}}{\lambda_{1} + \lambda_{2}}
$$
$X = min(X_{1}, X_{2})$, then $X \sim Exp(\lambda_{1} + \lambda_{2})$
[[inverse transform method]] (Generating random variables)
[[inequalities]]
1. [[Markov's Inequality]]
2. [[Reverse Markov]]
3. [[Chebyshev's Inequality]]
4. [[Chernoff Bound]]
	1. [[Sometimes Stronger Chernoff]]
	2. [[Chernoff Binomial]]
5. [[Hoeffding's Inequality]]
[[Tail Bounds and Applications]]
[[Confidence Intervals]]
[[CLT Theorem]]
CLT based approximate confidence interval
Say we are given $X_{1}, \dots, X_{n}$ and we only know that $Var(X_{i}) = \sigma^{2}$
$\bar{X}=\frac{X_{1} + \dots + X_{n}}{n}$
Let $\phi(.)$ be the cdf of the standard Normal [[Normal Distribution]], and 
$$
\phi\left( z \frac{\alpha}{2} \right) = 1 - \frac{\alpha}{2},\;  z \frac{\alpha}{2}=\phi^{-1}\left( 1- \frac{\alpha}{2} \right)
$$
Then $$
\left[\bar{X} - z \frac{\alpha}{2}\cdot \frac{\sigma}{\sqrt{ n }}, \bar{X} + z \frac{\alpha}{2}\cdot \frac{\sigma}{\sqrt{ n }}   \right] 
$$
is a $(1- \alpha)\cdot 100\%$ confidence interval for $\mathbb{E}\left[ X \right]$
[[with high probability]]
[[Balls and Bins whp]]



