if $X\sim U(0,1)$ then
[[p.d.f]]
$$
f_{X}(x) = \begin{cases}
	\frac{1}{b-a} & \text{if }a\leqslant x \leqslant b \\
	0 & \text{otherwise} \\
\end{cases}
$$
[[c.d.f]]
$$
	F_{X}(x) = \int_{a}^{x} \frac{1}{b-a} \, dt=\frac{x-a}{b-a} 
$$
[[tail]]
$$
	\bar{F}_{X}(x) = 1 - F_{X}(x) = 1 - \frac{x-a}{b-a}
$$

[[Expectation]], [[Expectation Uniform]]
$$
\mathbb{E}\left[ X \right] = \frac{a+b}{2}
$$
