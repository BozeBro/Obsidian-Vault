X,A,B are discrete random variables such that 
$$
X = \begin{cases}
A  & \text{w.p. } & p \\
B & \text{w.p } & 1 - p
\end{cases}
$$
Then $$
\hat{X}(z) = p \hat{A}(z) + (1-p)\hat{B}(z)
$$
$$
\begin{align}
	\hat{X}(z) & = \mathbb{E}\left[ z^{X} \right]  \\
& = \mathbb{E}\left[ z^{X} \mid X = A \right] \cdot p + \mathbb{E}\left[ z^{X} \mid X = B \right] (1-p) \\
& = \mathbb{E}\left[ z^{A} \right] \cdot p + \mathbb{E}\left[ z^{B} \right] \cdot (1-p) \\
& = p \hat{A}(z) + (1-p) \hat{B}(z)
\end{align}
$$