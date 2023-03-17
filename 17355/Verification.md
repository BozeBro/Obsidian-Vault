Goal: show program behaves in a certain way
[[Hoare Triples]]
We use Hoare Triples to see how to make assertions about a program to prove verification for the while3addr language.

$$
\begin{align}
	&\text{ skip } \frac{}{\vdash \left\{ P \right\} \text{ skip }\left\{ P \right\} }\\
	& \text{ assign } \frac{}{\vdash \left\{ \left[ \frac{a}{x} \right] P \right\}x=a\left\{ P \right\}  }\\
	& \text{ seq } \frac{\vdash \left\{ P \right\} S,\left\{ P' \right\} \vdash \left\{ P' \right\} S_{2}\left\{ Q \right\} }{\left\{ P \right\} S_{1},S_{2}\left\{ Q \right\} }\\
	& \text{ while } \frac{\vdash \left\{ P\wedge b \right\} C\left\{ P \right\} }{\vdash\left\{ P \right\} \text{ while b do c}\left\{ P\wedge \neg b\right\} }\\
	& \text{ consequence } \frac{\vdash P' \implies P \vdash \left\{ P \right\} S\left\{ Q \right\}  \vdash Q \implies Q'}{\vdash \left\{ P' \right\} S\left\{ Q' \right\} }
\end{align}
$$
In verification, we want the precondition to be as general as possible, and post condition to be as specific as possible.  OR
$$
\text{ Little Assump }code \text{ Many assumptions }
$$
#Strongest-Precondition
$$
\begin{align}
	&\text{ if }\left\{ P \right\} S\left\{ Q \right\} \wedge \forall Q' \text{ s.t. } \\
& \left\{ P \right\} S\left\{ Q' \right\} , Q\implies Q'  \\
&\text{ then } Q \text{ is the strongest precondition w.r.t. P}
\end{align}

$$
#Weakest-Precondition
	1. assign - wp(x=a,R) = $\left[ \frac{a}{x}R \right]$
	2. Seq wp(S,T,R) = wp(S, wp(T,R))
	3. If wp(if b then S else T, R) = 
		1. $b\implies wp(S,R) \wedge\neg b \implies wp(T,P)$

[[Examples for weakest Precondition P]]
Use loop invariants to prove stuff about pre and post conditions
$$
\left\{ P \right\} \text{ while }i < x; i = i+1 \left\{ i > 0 \right\}
$$
Loop Invariants have
1. $P \implies Inv$  (invariant holds at start of loop)
2. $\left\{ Inv \wedge b \right\}S\left\{ Inv \right\}$ (Invariant is preserved)
3. $\left\{ Inv \wedge \neg b \right\}\implies Q$ (Post holds after loop terminates)
[[Example Loop Invariant Proof]]

