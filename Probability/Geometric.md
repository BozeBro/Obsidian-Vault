
Given X is a Discrete [[Random Variable]], and lands on heads with probability p, we find
how many tails with probability $1-p$ we see before we see a head.
## [[Expectation]]
$$\mathbb{E}[X] = \frac{1}{p}$$
## [[p.m.f]]
$$p(i)=(1-p)^{i-1}p^i$$
## [[c.d.f]]
$$F(i) = 1 - (1-p)^i$$
## [[tail]] 
$$\overline{F}(i)=(1-p)^i$$
[[Variance]] and [[Variance Geometric]]
$$\frac{1-p}{p^2}$$
The Intuition is that the First i flips are tails.
Geometric is the only discrete distribution that is [[memoryless]]