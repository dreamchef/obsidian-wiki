
#analysis 

For each $n \in \mathbb{N}$ assume we are given a closed interval $I_n = [a_n,b_n] = \{x \in \mathbb{R} : a_n \leq x \leq b_n\}$.  Assume that each interval $I_n$ contains $I_{n+1}$.  Then it holds that
$$\bigcup\limits_{n=1}^\infty I_n \neq \emptyset$$

*Proof*:
Consider the set $A = \{a_n : n \in \mathbb{N}\}$ of left-hand endpoints of the intervals.  Clearly every $b_n$ serves as an upper bound for $A$.  Let real number $x = sup A$.
Now consider a particular $I_n = [a_n,b_n]$.  Because $x$ is an upper bound for $A$, we know $a_n \leq x$.  The fact that each $b_n$ is an upper bound for $A$ and that $x$ is the [[supremum]] implies that $x \leq b_n$.  So $a_n \leq x \leq b_n$ and an arbitrary small interval $I_n$ is nonempty, so the intersection is nonempty.

This directly implies the [[Bolzano-Weierstress Theorem]].