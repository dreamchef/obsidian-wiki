---
id: zlut2yi2ndwzl0jwr2surs6
title: Max Flow Algorithm
desc: ''
updated: 1656512637513
created: 1654530813357
---
#combinatorics 

1. Identify a directed path from [[source]] to [[sink]] in the graph such that every arc in the path has a strictly positive capcity.  This is an [[augmenting path]]  If no such path exists,  you are ***done***.
2. Identify the minimum capacity $\theta$ of this path.  Increase the flow in this path by $\theta$.
3. Decrease the *remaining* capacity of each arc on this path by $\theta$; increase the total flow by $\theta$.  ***Return*** to step 1.
