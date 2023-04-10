### #Z-Transforms
$$
\hat{X}(z) = \mathbb{E}\left[ z^{X} \right] = \sum z^{i}p(i)
$$
$\hat{X}(z)$ is bounded for any $\mid z \mid \leq 1$
$$
\hat{X}^{(n)}\mid_{z=1} = \mathbb{E}\left[ \prod_{0}^{n-1} (X-i) \right] 
$$
See [[z-transform-geometric]], [[z-transform-binomial]], [[z-transform-bernoulli]]
[[z-transform conditioning]], [[z-transform-random-sum]]
### #Laplace-Transforms 

^93e98f

$$
\tilde{X}=\mathbb{E}\left[ e^{-sX} \right] = \int_{0}^{\infty} e^{-st}f(t) \, dt  
$$
See [[Laplace-Exponential]], [[Laplace-Uniform]]. [[Laplace-Random-Sums]]

$$
\tilde{X}^{n}(s)|_{s=0} = (-1)^{n}\mathbb{E}\left[ X \right] 
$$

If $B(x)$ is a [[c.d.f]] and $b(x)$ is the [[p.d.f]] then
$\tilde{B}(s) = \frac{\tilde{b}(s)}{s}$


Linearity of z-transforms
If $X\bot Y, W= X+Y$, then ^abf9aa
$$
\hat{W}(z)=\hat{X}(z)\cdot\hat{Y}(z)
$$

