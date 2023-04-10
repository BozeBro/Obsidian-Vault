Let $T_{1}, T_{2},\dots T_{n} \dots$ be inter-event times of a seuqnece of events. (This is from [[2nd Poisson Process Def]])
$$
P(T_{1} > t) = \mathbb{P} \left\{ N(t) = 0 \right\} = \frac{e^{-\lambda t}(\lambda t)^{0}}{0!} = e^{-\lambda t}
$$
WTS $T_{i} \sim Exp(\lambda)$
$$
\begin{align}
	& \mathbb{P} \left\{ T_{n+1} \mid \sum_{1}^{n}T_{i} = s \right\}  \\
& = \mathbb{P} \left\{ 0 \text{ events in }  (s, s+t) \right\}\mid \sum_{1}^{n} T_{i} = s \\
& = \mathbb{P} \left\{ 0 \text{ events in }  (s, s+t)\right\} \text{ indpt increments} \\
& = e^{-\lambda t} \text{ stationary increments}
\end{align}
$$
