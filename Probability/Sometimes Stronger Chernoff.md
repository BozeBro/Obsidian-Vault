#Theorem18-6 
$$
X = \sum_{i=1}^{n}X_{i}\; X_{i} \text{ i.i.d}\; X_{i}\sim Bern(p_{i})
$$
$$
\mu = \mathbb{E}\left[ X \right] =\sum_{i=1}^{n}p_{i}\; \forall \epsilon > 0,
$$
$$\mathbb{P} \left\{ X \geqslant (1 + \epsilon)\mu \right\} < \left( \frac{e^{\epsilon}}{(1+\epsilon)^{1+\epsilon}} \right) ^{\mu} = (f(\epsilon))^{\mu}$$
f decreases as $\epsilon$ increases, therefore the bound is really good when $\epsilon$ grows to infinity.
When $0 < \epsilon < 1$,
$$
\mathbb{P} \left\{ X \leqslant (1-\epsilon)\mu \right\} \leqslant \left( \frac{e^{-\epsilon}}{(1-\epsilon)^{1-\epsilon}} \right) ^{\mu}
$$
[[Compare Sometimes Strong & Chernoff]]
