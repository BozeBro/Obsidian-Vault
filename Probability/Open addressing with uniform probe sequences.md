#Hashing 
We'll use n hash functions to uniformally probe the array.
$$
<h(k,1), h(k,2), h(k,3), \dots , h(k,n)>
$$
Idea is that there is less clustering than in [[Linear Probing]]
Load factor $\alpha = \frac{m}{n} < 1$
Expected cost of unsuccessful search is at most $\frac{1}{1-\alpha}$
[[Uniform search cost proof]]
