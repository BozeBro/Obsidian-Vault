Bound is also known as Pretty Chernoff bound for Binomial
See [[Binomial]] and [[Expectation Binomial]] and [[Variance Binomial]] and [[Proof Chernoff Bound for Binomial]], 
Also known as #Theorem18-4 

$$\forall \delta>0\, P(X-np\geqslant \delta)\leqslant e^{-2\delta^2/n}$$
$$P(X-np\leqslant -\delta)\leqslant e^{-2\delta^2/n}$$
See [[coin flip Chernoff]] for example
Subtleties:
1. If $d\in\Theta(n)$, (e.g. $\frac{n}{4}$) then the bound is in the form $e^{-\Theta \left( n \right)}$, which decreases with n. (strongest case of the bound)
2. If $d\in\Theta \left( \sqrt{ n } \right)$, then the bound is constant. Intuition: we are seeing how far we deviate by some standard deviation which is independent for high n. No stronger than [[Chebyshev's Inequality]] and converges to a constant via [[CLT Theorem]]
3. If $d\in\Theta \left( 1 \right)$, then the bound grows with n instead of shrink since the variance of [[Binomial]] grows with higher n, so the chances of being greater than a constant grows. (Weakest case of the bound)