
Given X is a  [[Random Variable]] $X \sim Poisson(\lambda)$, and expecting an average of $\lambda$ arrivals to a website per second, we can approximate the the number of arrivals are independent ([[independence]]) which each have a small probability.
## [[Expectation]]
$$\mathbb{E}[X] =\lambda$$
## [[p.m.f]]
$$p(i)=\frac{e^{-\lambda}\lambda^i}{i!}$$
## [[c.d.f]]
$$F(i)=\sum_0^ip(i)$$
## [[tail]] 
$$\overline{F}(i)=1-F(i)$$
Poisson(np) looks similar to [[Binomial]] for Bin(n,p) for small p and large n. Proof is at [[Poisson similar to Binomial]]
## [[Variance]] and [[Variance Poisson]]
$$\lambda$$
[[Poisson Process]] shows more qualities about the Poisson Process.

[[Chernoff Poisson]] Show's an upper bound on Poisson Tails.