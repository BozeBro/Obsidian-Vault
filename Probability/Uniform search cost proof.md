$$
\begin{align}
	& \mathbb{P}\left\{ X > 0 \right\}  \\
& \mathbb{P}\left\{ X > 1 \right\} =  \\
& \mathbb{P}\left\{ \text{First cell we look at is occupied} \right\} = \alpha   
\end{align}
$$
m occupied spots, and n possible spots.
$$
\begin{align}
	\mathbb{P}\left\{ X > 2 \right\} & = \mathbb{P}\left\{ \text{First tw cells are occupied} \right\}   \\
& \mathbb{P}\left\{ A_{1} \cap A_{2} \right\}    \\
& = \alpha \cdot \frac{m-1}{n-1} \\
& = \alpha \cdot \frac{\alpha n - 1}{n - 1} \\
& < \alpha \frac{\alpha n}{n} \\
& = \alpha^{2}
\end{align}
$$
We can generalize the rule here
$$
\begin{align}
	\mathbb{P}\left\{ X > i \right\}  & = \mathbb{P}\left\{ \text{First i cells are occcupied} \right\}  \\
  & = \mathbb{P}\left\{ A_{1} \cap A_{2} \dots A_{i} \right\}   \\
& = \mathbb{P}\left\{ A_{1} \right\} \mathbb{P}\left\{ A_{2} \mid A_{1} \right\} \dots \mathbb{P}\left\{ A_{i} \mid A_{1} \cap A_{2} \cap \dots \cap A_{i-1} \right\}     \\
& = \frac{m}{n} \cdot \frac{m - 1}{n - 1} \dots \frac{m - i + 1}{n - i + 1} \\
& \leqslant \alpha^{i}
\end{align}
$$
Then, with this information, we can upperbound the search cost expectation.
$$
\begin{align}
	\mathbb{E}\left[ X \right] & = \sum_{i=0}^{\infty}\mathbb{P}\left\{ X > i \right\}  \\
& = 1 + \sum_{i=1}^{n - 1}\alpha^{i} \\
& \leqslant \sum_{i=0}^{\infty} \alpha^{i} \\
& = \frac{1}{1 - \alpha}
\end{align}

$$