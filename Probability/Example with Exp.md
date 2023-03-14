[[Exponential]], [[c.d.f Exp]] is $F_X(x)=1-e^{-\lambda x}$
By [[inverse transform method]], we want 
$$
\begin{align*}
	x & = F^{-1}(u)\\
	F(x) &= u\\
	1-e^{-\lambda x} & = u\\
	-\lambda x = ln(1- u)\\
	x & = -\frac{1}{\lambda}ln(1- u)
\end{align*}
$$
Given $u\in U)0,1)$, setting $x=1\frac{1}{\lambda}ln(1-u)$ produces an instance of $X\sim Exp(\lambda)$
