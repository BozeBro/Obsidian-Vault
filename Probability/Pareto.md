$X \sim \text{Pareto}(\alpha)$ if 
$$
\bar{F_{X}}(x) = \mathbb{P} \left\{ X > x \right\} = x^{- \alpha}, \forall x \geq 1,\, 0 < \alpha < 2
$$
For $0 < \alpha < 1$, the [[Expectation]] and [[Variance]] grow infinitely large, otherwise the Expectation and Variance are finite. The higher [[kth Moment]] are still infinite.

Bounded Pareto Distribution
Useful for when data lies in a certain boundary or dealing with empiral samples.
$X \sim \text{Pareto}(k,p,\alpha)$ then
$$
f(x)\equiv \alpha x ^{-\alpha - 1}\cdot \frac{k^{\alpha}}{1-\left( \frac{k}{p} \right)^{\alpha}}
$$
where $k \leq x \leq p$ and $0 < \alpha < 2$
Pareto has the properties
1. Decreasing failure rate (DFR) - more CPU used implies more CPU usage will be used.
2. Infinite or near-infinite variance
3. "Heavy-Tail" - A small fraction of jobs take up at least 50% of the work load. 
	1. Note, [[Exponential]] has constant failure rate (since it is [[memoryless]])
4. 