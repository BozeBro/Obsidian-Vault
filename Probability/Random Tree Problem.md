An example from textbook is a tree whose leaves sprout two children with probability one half, and we want to know the total number of leaves in the tree after t steps. The number of leaves is totally random since we can gain 1 or 2 leaves at each time step.

Note, we can say at $X_t$, we know that for the previous branch, the leaves of $X_{t-1}$, we contribute 1 or two leaves.
Therefore,
$$X_t=\sum_1^{X_{t-1}}Y_i$$
where $Y_i$ is a leaf with equal chance of giving 1 or 2 children. We have a [[Random Sums]]
Note, each Y is independent of each other and $X_{t-1}$ is independent of the leaves [[independence]]
Problem is much easier to solve now, and is left as an exercise for reader
Answer should be $(\frac{3}{2})^t$ for [[Expectation]] and $(\frac{9}{4})^t\frac{1}{3}(1-(\frac{2}{3})^t)$ for [[Variance]]