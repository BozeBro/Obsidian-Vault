$Var(X)=p(1-p)$
See [[Bernoulli]] for additional information on Bernoulli
For conditioning,
$$\begin{align*}
Var(X) & = E[(X-p)^2]\\
& = E[(X-p)^2 | X = 1]*p + E[(X-p)^2 | X = 0]*(1-p)\\
& = (1-p)^2\cdot p + p^2(1-p)\\
& = p(1-p)
\end{align*}$$
Linearity of Variance occurs only when X and Y are independent
$Var(X+Y)=Var(X)+Var(Y)$