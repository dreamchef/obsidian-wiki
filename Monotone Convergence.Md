
#analysis 

If a sequence is [[monotone]] and [[bounded]], then it is [[converge]]nt.

*Proof:*
Let $(a_n($ be [[monotone]] and [[bounded]].  Assume it is [[increasing]] and consider the set of points $\{a_n: n\in\mathbb{N}\}$.  Let $\lim a_n =s = \sup\{a_n: n \in\mathbb{N}\}$.
Now let $\epsilon > 0$.  Because $s$ is the [[supremum]], we know $s-\epsilon$ is not an upper bound, so there exists a point in the sequence $a_N$ such that $a-\epsilon < a_N$.  Now because $(a_n)$ is increasing, $n \geq N \implies a_N \leq a_n$.  Altogether,
$$s-\epsilon < a_N \leq a_n \leq s < s + \epsilon$$
which implies $|a_n - s| < \epsilon$, as desired.
