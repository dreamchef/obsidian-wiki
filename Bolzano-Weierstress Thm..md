---
id: 1uoe2lsgjhzrdhx9qlb98fi
title: Bolzano-Weierstrauss Theorem
desc: ''
updated: 1656438230679
created: 1654530814100
---
#analysis

Every [[bounded ]] [[sequence]] contains a [[converge]]nt [[subsequence]].

This directly implies the [[Cauchy Condensation Test]].

*Proof*: Let $(a_n)$ be a bounded sequence with upper bound M.  Bisect the closed interavl $[-M,M]$ into two closed intervals $[-M,0]$ and $[0,M]$.  Now it must be that at least one of these closed intervals contains an infinite unmber of the terms in the squence $(a_n)$.  Select a half for which this is the case and label it $I_1$.  Then, let $a_{n_1}$ be some term in the sequence satisfying $a_{n_1} \in I_1$.  Next, we bisect $I_1$ into closed intervals of equal length andl et $I_2$ be a half that again contains an infinite number of terms of the original sequence.  Now we can select a term $a_{n_2}$ with $n_2 > n_1$ where $a_{n_2} \in I_2$.  In general, we construct the closed interval $I_k$ by taking a half of $I_{k-1}$ containing an infinite number of terms of $(a_N)$ and then select $n_k>n_{k-1}>...>n_1$ so that $a_{n_k} \in I_k$.
Now we want to argue that $(a_{n_k})$ is a convergent subsequence, but we need a candidate for the limit.  The sets

$$I_1 \subseteq I_2 \subseteq I_3 \subseteq ...$$

form a nested sequence of closed intervals, and by the [[Nested Inverval Property]] there exists at least one point $x \in R$ contained in every $I_k$.  With $x$ as our candidate, let $\epsilon > 0$.  By construction, the length of $I_k$ is $M (\frac{1}{2})^{k-1}$ which converges to zero.  Choose $N$ so that $k \geq N$ implies that the length of $I_k$ is less than $\epsilon$.  Because $x$ and $_{n_k}$ are both in $I_k$, it follows that $|a_{n_k}-x| < \epsilon$.
