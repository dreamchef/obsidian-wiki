
#combinatorics  #problem

Consider alphabet set $\Sigma$ and all words of length $n$ from $\Sigma$ (cardinality $|\Sigma|^n$). Create some sequence that contains every word at least once (wrap-around words allowed).
# Solution
1. Create a digraph D where
	- each vertex is a word of length $n-1$
	- between each two vertices with words $b_1b_2...b_{n-1}$ and $b_2b_3...b_n$, there is an edge with word $b_1b_2...b_n$.
2. Find an [[eulerian chains & paths|eulerian closed path]].
3. The sequence comprises the first letter from each vertex in the path, in order.
