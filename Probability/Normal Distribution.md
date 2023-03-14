[[Central Limit Theorem]] 
[[Standard normal]]
It is a good way to approximate a large number of independent, equally distributed sources.

[[p.d.f]]
$$\forall -\infty < x < \infty\; f_X(x)=\frac{1}{\sqrt{2\pi}\sigma}e^{-\frac{1}{2}\left(\frac{x-u}{\sigma}\right)^2}$$

$X\sim N(\mu, \sigma^2)\implies E[X] = \mu\land Var(X)=\sigma^2$
Normal Distributions also have a special property in that they act linearly.
[[Linear Transformation Property]]
There is also a theorem relating a Normal Distribution to its Standard Normal variation.
### Theorem 9.8
If $X\sim N(\mu,\sigma^2)$, then the probability that X deviates from its mean by less than k standard deviations is the same as the prbability that the [[Standard normal]] deviates from its mean by less than k.
$$Y =\frac{X-\mu}{\sigma}\sim N(0,1)\land X\sim N(\mu,\sigma^2)
$$
$$P(-k\sigma<X-\mu<k\sigma)=P(-k<\frac{X-\mu}{\sigma}<k)=P(-k<Y<k)$$
