---
id: w9ntvb6c3t0mtxy7qp9fc5i
title: Matrix Multiplication
desc: ''
updated: 1656512630687
created: 1654530813340
---
#linear-algebra #concept 

Each entry in *C* is the [[dot product]]s of a row in *A* with a column in *C*.

Matrix multiplication is associative, but not (necessarily) commutative.
# Computation
Consider $AB = C$. There are multiple ways to obtain $C$.

1. Each of the column of $C$ is the matrix $A$ multiplied by a column of $B$.

2. Alternatively, the rows of *C* are rows of *A* multiplied by the matrix *B*
![](https://miro.medium.com/max/697/1*4dIpYSmMCDKkmnyvuJCdMQ.png)
3.  The matrix *C* is the sum of matrices that are columns of *A* multiplied by rows of *B*.
![](https://miro.medium.com/max/700/1*6-PSPcjj58axx6MZ1D3feg.png)
