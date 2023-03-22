Let $T_{1}$ denote the time of the one event.
$$
\begin{align}
	\mathbb{P} \left\{ T_{1} < s \mid N(t)=1 \right\} & = \frac{\mathbb{P} \left\{ T_{1}<s \wedge N(t)=1 \right\} }{\mathbb{P} \left\{ N(t) = 1 \right\} } \\
	& = \frac{\mathbb{P} \left\{ \text{1 event in }  \left[ 0,s \right] \right\}\wedge \text{0 events in }\left[ s,t \right] }{\frac{e^{-\lambda t(\lambda t)^{1}}}{1!}} \\
	& = \frac{\mathbb{P} \left\{ \text{1 event in }  \left[ 0,s \right] \right\}\mathbb{P} \left\{ \text{0 events in } \right\} \left[ s,t \right] }{e^{-\lambda t}\lambda t} \\
	& = \frac{e^{-\lambda s}\cdot\lambda s \cdot e^{-\lambda (t - s)} \cdot (\lambda (t - s))^{0} }{e^{-\lambda t}\lambda t } \\
	& = \frac{s}{t}
\end{align}
$$