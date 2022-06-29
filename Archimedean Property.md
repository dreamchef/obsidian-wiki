
#analysis
## Part One
Given any real number $x$ there exists an $n \in \mathbb{N}$ satisfying $n > x$.

*Proof*: Assume that $N$ is bounded above.  By athe [[axiom of completeness]] $N$ should have a [[supremum]], and we can set $\alpha = sup \mathbb{N}$. If we consider $\alpha - 1$ we no longer have an upper bound so there exists an $n \in. \mathbb{N}$ s.t. $\alpha - 1 < n$.  But this is equivalent to $a < n + 1$.  Because $n + 1 \in \mathbb{N}$, $\alpha$ is not an upper bound which contradicts our supposition that $x = sup N$.
## Part Two
Given any real number $y > 0$, there exists an $n \in \mathbb{N}$ s.t. $1/n < y$.

*Proof:* Let real number $x = 1/y$ where $y$ is a positive real number.  By part one, there exists $n \in \mathbb{N}$ s.t. $n > 1/y$.  This is equivalent to $1/n < y$.
