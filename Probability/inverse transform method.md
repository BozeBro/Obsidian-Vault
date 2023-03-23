### Algorithm
1. Generate $u\in U(0,1)$
2. Return $x\in F^{-1}_X(u)$

[[Example with Exp]]
### Assumptions
1. We have the [[c.d.f]] of X
2. We can get x from the [[c.d.f]]
3. We have a generator for [[Uniform]]
## [[Continuous inverse transform method]]
Assume $0<X<n, n > 0$.
When getting a random number, we want to map $u\to x$ where u is in the codomain of F ([[c.d.f]]) and x is in the domain.
$$u=F_X(x)\; x=F^{-1}_X(u)$$
So the function to generate random numbers will be drawn from g where $g = F$

## [[Discrete inverse transform method]]
