
#combinatorics 

Given n workers and m jobs, and performance ratings $r_{ij}$, and adjacency $x_{ij}$ for worker i and job j; find a fully saturated, maximum-weight (total performance rating) matching.
Maximize the summation:
$$\sum_{i=1}^n\sum_{j=1}^mr_{ij}x_{ij}$$

Note that $\sum_{i=1}^nx_{ij} = 1$ and $\sum_{j=1}^mx_{ij} = 1$.
