Assume $0<X<n, n > 0$. and X is a [[Random Variable]]
When getting a random number, we want to map $u\to x$ where u is in the codomain of F ([[c.d.f]]) and x is in the domain.
$$u=F_X(x)\; x=F^{-1}_X(u)$$
So the function to generate random numbers will be drawn from g where $g = F$
### Algorithm
1. Generate $u\in U(0,1)$
2. Return $x\in F^{-1}_X(u)$
