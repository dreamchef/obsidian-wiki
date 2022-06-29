---
id: tnhc85rp3zodv8bgmp2ah28
title: Markov Matrix
desc: ''
updated: 1656470495867
created: 1654530813292
---
#linear-algebra 

matrix A with the following properties
1. Every entry of A is positive: $a_{ij} > 0$
2. Every column of A sums to 1

The steady-state vector $u_{\infty}$ resulting from left-multiplying a positive vector $u_0$ many times by A, is equal to the eigenvector $x_1$ corresponding to the eigenvalue value $\lambda_1 = 1$. Equivalently, 
raising matrix to a very high exponential gives equilibrium.

Rows are to-states and columns are from-states. Each entry is the probability of a state transition. For example, columns and rows might represent rooms. So entries represent probability of agent moving between rooms.

Markov matrices are used to represent systems where only current position, not history, matters.
