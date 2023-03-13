
Given X is a  [[Random Variable]] and n [[Bernoulli]] variables, or flipping n biased coins with probability p, we want to see x coins land on heads. Each coin flip is independent [[independence]]
## [[Expectation]]
$$\mathbb{E}[X] = np$$
## [[p.m.f]]
$$p(i)={n\choose i}p^i(1-p)^{n-i}$$
## [[c.d.f]]
$$F(i)=\sum_0^ip(i)$$
## [[tail]] 
$$\overline{F}(i)=1-F(i)$$
For large n, and small probability p, Bin(n,p) looks like the [[Poisson]] Poisson(np) the proof can be found at [[Poisson similar to Binomial]]
For variance see [[Variance Binomial]]