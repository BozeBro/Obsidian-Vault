[[Poisson Process]] has rate $\lambda$
Follows
1. N(0)=0
2. Process has [[Independent Increments]]
3. $$\forall s,t\; P(N(t+s)-N(s)=n)=\frac{e^{-\lambda t}(\lambda t)^n}{n!}$$
Rule 3 implicitly uses [[stationary Increments]]
See [[2nd Poisson Process Def]] to see how we relate the time of a Poisson Process
Inuitions: When seeing
$$P(N(x) = n\mid N(x+t) = n+m)$$
We are actually just asking for the probability that we see n arrivals in x seconds, and m arrivals in $[x,x+t]$.