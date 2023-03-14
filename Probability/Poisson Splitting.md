X is [[Poisson Process]] with rate $\lambda$ We label each arrival as A or B with probabilities p, 1-p respectively. 
Type A events form [[Poisson Process]] with rate $p\lambda$ and B has [[Poisson Process]] with rate $(1-p)\lambda$ and A,B are [[independent]]

$$P(N_A(t)=n,N_B(t)=m)=P(N_A(t)=n)P(N_B(t)-m)$$
$$= e^{-\lambda tp}\frac{(\lambda tp)^n}{n!}e^{-\lambda t(1-p)}\frac{(\lambda t(1-p))^n}{n!}$$
See [[N(t) Number of arrivals by time t]] to get its distribution
