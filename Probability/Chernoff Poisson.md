[[Chernoff Poisson Derivation]]
$$E[e^{tX}]=e^{\lambda(e^t-1)}$$
If $a > \lambda$ 
$$P(X\geqslant a)\leqslant min_{t>0}e^{\lambda(e^t-1)-ta}$$
Expression is minimized when $t=ln(\frac{a}{\lambda})$
$$P(X\geqslant a)\leqslant e^{a-\lambda}\left(\frac{\lambda}{a}\right)^a$$

See [[Poisson]] for more information