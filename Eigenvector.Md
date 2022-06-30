
#linear-algebra #concept
# Computation
To find the Eigenvector $\vec{v}$ associated with [[Eigenvalue]] $\lambda$, consider the equation
$$(A - \lambda I_n)\vec{v} = 0$$
Represent the equation as an augmented matrix in [[RREF]] to find the components of the Eigenvector.
# Statements
1. Let A be an n by n matrix with corresponding linear function $L_A: R^n \rightarrow R^n$. The [[vector space]], $K \subset R^n$, of all Eigenvectors in A associated with a nonzero Eigenvalue combined with the zero vector forms an [[invariant]] subspace of $R^n$
2. Let A be an n by n matrix with real, distinct Eigenvalues ordered by magnitude in decreasing order.  If the magnitude of the first (highest-magnitude) Eigenvalue is 1, then for any $\vec{x} \in R^n$, iterative application of the matrix mapping to $\vec{X}$ yields a vector approaching the Eigenvector $\vec{v}_1$ associated with $\lambda_1$. $$A^k\vec{x}\rightarrow \vec{v}_1 \,\, as \,\, k \rightarrow \infty$$
3. When A is squared, the Eigenvalues stay the same.
4. #q symmetric matrices and orthogonal E-vals? related to [[singular value decomposition]]
5. The fact that two matrices have the same Eigenvalues does not imply they have the same Eigenvectors
6. The Eigenvectors are unchanged if $I$ is added to the matrix.
