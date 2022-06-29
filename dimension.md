---
id: 08hxv23dp5tqzltzlnckylq
title: Dimension
desc: ''
updated: 1656451268346
created: 1654530812878
---
#linear-algebra

Vector space $V$ has finite dimension if it is the span of a finite number of vectors.  If $V$ has finite dimension, then the fewest number of vectors that span $V$ is called the [[dimension]] of $V$ and is denoted dim($V$).  Alternatively, the dimension is equal to the cardinality of all [[basis]] sets for V.

# Properties
- If $W$ is a [[basis]] matrix, then $dim(W) = rank(W) = rank(W^T)$ ([[rank]])
- Let $V$ be a vector space of dimension $n$, and let $\{\vec{v}_1, \vec{v}_2, ... , \vec{v}_k\}$ be a set of vectors in $V$.  The following implications hold when they apply
	1. If $\{\vec{v}_1, \vec{v}_2, ... , \vec{v}_k\}$ is a [[linearly independent]] set, then $k \leq n$
	2. If $k /leq n$, then $\{\vec{v}_1, \vec{v}_2, ... , \vec{v}_k\}$ is a [[linearly dependent]] set.
- Let $W$ be a subspace of a finite dimensional vector space $V$.  The following implications hold when they apply
	1. If $W$ is a proper subspace, then $dim(W) < dim(V)$
	2. If $dim(W) = dim(V)$, then $W = V$
- Let $B = \{\vec{v}_1, \vec{v}_2, ... , \vec{v}_n\}$ be a set containing $n$ vectors in a $n$-dimensional vector space $V$.  TFAE:
	1. $B$ is a [[span]]ning set of $V$
	2. $B$ is a [[basis]] for $V$
	3. $B$ is a [[linearly independent]] set.
