#Hashing 
#### Load factor 
- hash table that stores m keys within n buckets
$$
\alpha = \frac{\text{Number keys}}{\text{Number buckets}} = \frac{m}{n}
$$
[[Simple Uniform Hashing Assumption]]
[[Separate Chaining]]

Under SUHA and separate chaining, if $m \geqslant 2n \ln n$, and $n$ buckets, then let $X$ be largest bucket size
$$
\mathbb{P} \left\{ X < e \alpha \right\} \geqslant 1 - \frac{1}{n}
$$
where $\alpha = \frac{m}{n}$
[[with high probability]]
See [[SUHA whp proof]]

[[Linear Probing]]
[[Open addressing with uniform probe sequences]]

