
#linear-algebra 

$$X = U\Sigma V^T$$, used to find the most important rank-1 matrices

This decomposition is gauranteed to exist, is unique, and does not require a square matrix.

All linear transformations can be decomposed into [ rotation ][ scaling ][ rotation ].
# Algorithm to Find $U\Sigma V^T$
1. Finding $\Sigma$
	1. Find [[Eigenvalue]]s of $A^TA$ or $AA^T$ (they give the same result except zeros)
	2. $\Sigma$ contains the singular values (square roots of Eigenvalues above) along main diagonal in nonincreasing order.
2. The columns of $U$ are the [[Eigenvector]]s of $AA^T$.
3. The rows of $V^T$ are the [[Eigenvector]]s of $A^TA$.
# Approximating $X$
1. Write the decomposition as a sum $\sigma_1u_1v_1^T + \sigma_2u_2v_2^T + ... + \sigma_mu_nv_m^T + 0$ where $n$ is the number of important columns from the "economy" form and $m$ is the number of important singular values.  See intuition for [[matrix multiplication]].
2. Choose a number of the terms (starting from the left) to get desired accuracy.

The **Eckard-Young Theorem** gaurantees that a sum as described above with $k$ terms is the best possible rank $k$ approximation of the matrix

## Application to image compression
This is the best method of low-rank matrix approximation and generates compressed images with minimal information loss.
