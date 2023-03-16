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
In verification, we want the precondition to be as general as possible, and post condition to be as specific as possible.