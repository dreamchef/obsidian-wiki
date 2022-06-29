---
id: vtu4ums6jwfeq7vr2nhxqgy
title: Eigenvalue
desc: ''
updated: 1654530811761
created: 1654530811761
---
#linear-algebra #concept
only defined for square matrices

Let A be an n by n matrix, then $\lambda \in C$ is an Eigenvalue of A if their is a nonzero vector $\vec{v} \in C^n$ such that
$$A\vec{v} = \lambda\vec{v}$$
The nonzero vector $\vec{v}$ is called an [[Eigenvector]] associated with the Eigenvalue $\lambda$.
Note: $\lambda$ is an Eigenvalue of A iff $(A-\lambda I)$ is singular
# Computation
Let A be an n by n matrix, then $\lambda \in C$ is an Eigenvalue of A if it satisfies $det(A-\lambda I_n) = 0$

# Products of matrices

# Properties
1. A and B share the same n [[linearly dependent]] eigenvectors if and only if AB = BA
2. If A and B are [[symmetric]], then the Eigenvalues are real and perpendicular.
3. **TFAE**
	- A has at least one zero Eigenvalue
	- det(A) = 0
	- A is [[singular]]
4. Every real-valued n by n matrix A has exactly n Eigenvalues. Moreover,
	1. $p_A(\lambda) = (\lambda - \lambda_1)(\lambda - \lambda_2)...(\lambda - \lambda_n)$
	2. det(A) = $\lambda_1\lambda_2...\lambda_n$
5. For n by n matrix A:
	1. A is singular iff 0 is an Eigenvalue of A
	2. If A is singular, then null(A) is the span of all Eigenvectors associated with $\lambda = 0$
	3. When A is squared, the Eigenvalues are squared.
	4. When we multiply an Eigenvector by A, it is multiplied by its Eigenvalue.
6. The fact that two matrices has the same Eigenvalues does not imply they have the same Eigenvectors
7. If $\lambda$ is an eigenvalue of $A$
	1. $\lambda^2$ is an eigenvalue of $A^2$
	2. $\lambda^{-1}$ is an eigenvalue of $A^{-1}$
	3. 	$\lambda + c$ is an eigenvalue of $A + cI$
