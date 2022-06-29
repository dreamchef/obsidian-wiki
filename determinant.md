
#linear-algebra
only defined in terms of square matrices
# Computation
## Triangular matrix
Given triangular matrix, determinant is product of the diagonal entries
## Cofactor method
sum of the products of the elements and their associated [[cofactor]]s along any row or column in the matrix
$det(A) = \sum_{i=1}^n a_{iq}C_A(i,q)$ for any column q
$det(A) = \sum_{j=1}^n a_{pj}C_A(p,j)$ for any row p
## Using [[REF]]
given a finite number of matrices $E_i$ such that
$$E_kE_{k-1}...E_1A = U$$
Based on [[determinant#^d0e945|determinant inverse theorem]], and the invertibility of elementary matrices #q what's happening this step
$$det(A) = \frac{1}{det(E_1)det(E_2)...det(E_k)}$$
# Properties
## Square matrix lemma
Given a square, $n$ by $n$ matrix A
1. Let $c \in R$, then det(cA) = $c^ndet(A)$
2. $det(A^T) = det(A)$
3. If any single row or single column of A is the zero vector, then det(A) = 0
4. Let a new matrix C be created by swapping any two rows in A, then $det(C) = -det(A)$
5. Let a new matrix D be created by swapping any two columns in A, then $det(D) = -det(A)$
## [[Elementary Matrix]] lemma
1. The determinant of a matrix that swaps two rows is -1.
2. ...that multiplies a row by a scalar $c$ is $c$.
3. ...that adds a multiple of one row to another row is 1.
### Corollary
1. If two rows are interchanged, the determinant changes sign
2. If multiplied by scalar determinant = determinant * scalar
3. If a multiple of one row is added to another, the determinant does not change
## Product theorem
If A and B are both n-by-n matrices, then det(AB)=det(A)det(B)
## Inverse determinant theorem

^d0e945

If A is an n-by-n [[invertible]] matrix, then $det(A^{-1})=\frac{1}{det(A)}$
### Corollary
An n-by-n matrix A is invertible iff $det(A) \neq 0$
